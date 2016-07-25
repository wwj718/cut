# todo
*  写成package包，使用pip安装，提供系统指令

---

###自动截图并上传到七牛的脚本
####依赖安装
* 确保pngpaste工具存在，如果不存在，可以通过brew安装，如果没有brew，请google关键字mac+brew
* brew install pngpaste

####使用方法
* 登陆七牛，如果你没有七牛账号，请注册
* 在账号设置页面，找到密钥标签，获取到AK和SK
* 新建一个空间，在空间设置页面，获取到您的域名
* 打开main.py，替换AK和SK，替换bucket为你的空间名，替换domain为你的域名
* 运行main.py，如python main.py，可以传一个参数，标记pngpaste绝对路径
* 按住command+ctrl+shift+4键，进行截图，也可以选择其他的截图工具，如QQ，只要这个截图工具截完图把图片放到剪切板就可以。
* 截图完成后，使用command+v即可以获取到url

####注意
* 目前只支持上传到七牛
* 有时候command+v无法获取到url，那么请等一会，具体取决于您的网速
* 目前在mac测试通过，理论上可以运行pngpaste系统都可以
