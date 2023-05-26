# 🤺 如果我从脚手架掏出这些功能，阁下该如何应对？

# 前言

> 由于最近公司的小项目比较多，又刚好落到我头上，所以只能临时抱佛脚疯狂`create vite`创建新项目，但是佛脚抱多了佛祖也嫌恶心(我瞎说的佛祖别怪我 🐶)，就萌生了自己撸一个脚手架的想法。偏偏我又是一个天马行空(屁事多)的人，于是在我边写边创作的过程中，写出来的"脚手架"也在逐渐偏离它原本的职责...

# 功能展示

## 新建

### `Create Project`

当然，在开头这个脚手架的方向还是非常正常的，由于公司的项目统一都使用`Vite`，因此我也将`Vite`作为我脚手架模板的框架，同时加上了`uniapp`版本

下面是`create project`功能的具体逻辑 👇 ![Create-Project.excalidraw](https://johnson-huang-pic-1312790691.cos.ap-guangzhou.myqcloud.com/webp_images/Create-Project.excalidraw.webp)

其中`johnson-hooks`、`johnson-utils`和`johnson-styles`是我平时写自己项目或者是工作中常用的一些方法和 hooks，也作为选装项放入创建项目功能中

> 由于这个功能比较常见，在此就不做演示了

### `Create Module`

> 这个命令会帮助你在当前目录下创建一个文件夹或文件，目前文件的可选类型有`Vue`和`TS`，如果选择`Vue`文件则会帮你初始化一份`Vue3 setup TypeScript`版本的.Vue 文件

## 服务

### `Server Open`

> 这个命令是我在日常工作中使用的最多的，它可以帮助你将`package.json`文件中`scripts`的命令全部列出来，然后选择需要启动的服务即可，简直就是我这种懒癌患者的福音! ![server-open](https://johnson-huang-pic-1312790691.cos.ap-guangzhou.myqcloud.com/raw_images/server-open.gif)

### `Server Start`

> 如果你需要在本地起一个临时的 node 服务器来做后端时，这个命令会帮到你。只需要输入一个可用端口，脚手架会帮你在`当前目录下`新建一个`JS文件`，为你初始化好 node 服务的最基本配置并在输入的端口上启动该服务 ![server-create](https://johnson-huang-pic-1312790691.cos.ap-guangzhou.myqcloud.com/raw_images/server-create.gif)

### `Server Port`

> 忘记`Windows怎么查看端口占用了?`无所谓，`fly`会出手！只需要输入`fly server port`即可查看本机被占用的端口 ![server-port](https://johnson-huang-pic-1312790691.cos.ap-guangzhou.myqcloud.com/raw_images/server-port.gif)

### `Server Kill`

> 如果你想直接关闭某个端口的进程，使用`fly server kill <port>`就可以帮你完成 ![server-kill](https://johnson-huang-pic-1312790691.cos.ap-guangzhou.myqcloud.com/raw_images/server-kill.gif)

## 删除

### `Delete <fileName>`

> 使用`fly delete <fileName>`并确认后即可删除`当前目录下`的某一文件(请谨慎使用！)

## 翻译

### `Translate`

> 是的你没有看错，`fly`脚手架甚至还有翻译功能，输入`fly translate`即可进入选择目标语言界面，确认后即可进入连续对话的翻译页面  
>  **当输入框为空时`输入回车`，即可重置目标语言**  
>  **同时，`fly`的翻译基于语言判断实现，意味着你可以输入任何类型的语言并将其转换成你想要的语言** ![translate](https://johnson-huang-pic-1312790691.cos.ap-guangzhou.myqcloud.com/raw_images/translate.gif)

## 计时

### `Countdown`

> 如果你需要有一个倒计时软件来帮助你管理时间，`fly`也能做到，只需要输入`fly countdown`，并输入倒计时名称以及倒计时时间(支持输入秒和`HHHH:MM:SS`为格式的时间)，即可开启倒计时，当倒计时结束，`fly`会在桌面给你发送通知 ![countdown](https://johnson-huang-pic-1312790691.cos.ap-guangzhou.myqcloud.com/raw_images/countdown.gif)

## 待完成功能

- [ ] NBA 赛事查询(当天)
- [ ] NBA 赛事查询(比赛详情)
- [ ] 压缩文件 ...

# 后记

感谢你看到这里，`fly`脚手架目前只是我开发的一个小玩具，但希望有一天它可以真的成长为一个成熟的脚手架。如果你有任何有趣的功能推荐，或者说对`fly`脚手架的功能有任何建议的话，欢迎到评论区留言，感激不尽

> 对了，如果你想下载`fly`脚手架，使用`npm i -g johnson-cli`下载即可
