# 说明
这里用于收集对本书的反馈，包括错别字以及技术错误等。如果您有各类反馈，请点Issues标签，提交issue，以便进行跟踪。

请注意：本repo中不回答与本书无关的问题，并会予以删除。如需求助请加如下qq群：

- Angular中文社区：
    - 一群：278252889（2000人群，将近满员）
    - 二群：305739270
    - 三群：207542263
    - 四群：454120058
- Angular互助组：200242234
- ionic开发实践：110455272

获得最新消息，请关注微信号“双狼说”

# 重要通知

一些读者反映安装FrontJet有困难，我做了一些改进，它支持在Node 5下运行。由于Node 5.x 版本的NPM工具有了显著提升，所以安装到一半儿被卡住等问题都解决了。请获取最新版FrontJet源码，并在它的目录下运行npm link。但是仍然需要翻墙，因为phantomjs的下载源被墙了。

部分书友反映安装front-jet失败，这是因为fj依赖了很多第三方库，安装时容易出现问题，特别是网络不好的时候。所以我制作了Windows下的离线安装包，链接: <http://pan.baidu.com/s/1mgZ3FMK>，密码: q5v5。先确保本地的NodeJS是4.x版本（注意：离线安装包不支持其它版本的NodeJS），然后把它解压到一个目录，然后把这个目录加入环境变量PATH中即可 —— 注意，添加完PATH之后要重新开cmd窗口才会生效。

如果安装后运行时出现`The 'libsass' binding was not found`错误，请进入`node_modules/gulp-sass`目录，然后运行`npm rebuild node-sass`即可。

另外，安装front-jet对于阅读不是必须的，它只是用来运行范例代码的环境工具。

# 勘误

## 关于Angular2的勘误
Angular开发组原本宣称只支持 IE11+，在本书定稿后已经把兼容性起点设置为IE9了，这意味着等它正式发布的时候，将可以完全替代现在的Angular 1.3的应用场景。

不过，如果需要支持IE8，那么仍然只能使用Angular 1.2。

## 部分电子版的勘误
有些电子版中把命令中的空格丢掉了，如`npm install-g`，应该为`npm install -g`，如果发现命令无法直接粘贴查看，请查查是否遗漏了空格。

## P252
`angular.module('com.ngnice.app').controller('demoService',function(){});`
应该改为：
`angular.module('com.ngnice.app').service('demoService',function(){});`

感谢网友`iceconfig`的指正！

## P20

两处`$urlRouterProvider.state(`应改为`$stateProvider.state(`。均为笔误。

感谢网友`ltyely`的指正！

## P12

第一行cpnm 应为cnpm，为笔误。

感谢网友`sally2015`的指正！

## P208

ng-bing 应为 ng-bind
