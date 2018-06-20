## Gitea服务的进阶配置

之前通过网页进行安装只是对Gitea服务端进行了简单的配置，
Gitea服务器本身还有不少进阶的配置可以设置。
自定义内容包括：配置文件、自定义ignore文件、自定义网页模板等内容！

### 定制自己的配置文件
要配置服务器首先需要找到服务器的配置文件，文件路径如下`D:\Gitea\custom\conf\app.ini`(**如果你使用了我之前设置的Gitea路径，用其他路径的我相信你能找到\^-\^**)
修改时需找到对应的键值对进行修改。

该文件的默认情况请查看[app.sample.ini](./app.sample.ini)，本文中没有提及的设置方式可以自行根据默认文件和需求情况自行修改。

#### 配置使用离线模式（能够显示随机生成的图像！）

找到`server`中的`OFFLINE_MODE`设置为**true**如下：

``` ini
[server]
OFFLINE_MODE = true
```

#### 解除上传附件限制
设置不限制上传的文件类型和文件大小为2GB。

附件可以上传到工单或者进行相关的版本发布！
``` ini
[attachment]
; 是否允许上传附件. 默认是`true`
ENABLED = true
; 附件保存的路径. 默认是`data/attachments`
PATH = data/attachments/:USER
; 允许上传的文件类型 
ALLOWED_TYPES = *.*
; 文件的最大大小. 默认是4MB
MAX_SIZE = 2048
; 每次上传文件的最大个数. 默认是5
MAX_FILES = 10
```


