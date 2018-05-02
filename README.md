# CodeHighlighter-for-Typecho

基于 prismjs 的代码语法高亮插件 for Typecho，可显示语言类型、行号，有复制代码到剪切板功能。

github开源地址：[https://github.com/Copterfly/CodeHighlighter-for-Typecho][1]

## 起始

本插件是基于 [prismjs][2] 的 `Typecho` 代码语法高亮显示插件。( Typecho 1.1版可用，其它版本请自行尝试)

可显示语言类型、行号，有复制功能。(请勿与其它同类插件同时启用，以免互相影响)

## 使用方法

第 1 步：下载本插件，解压，放到 `usr/plugins/` 目录中；

第 2 步：文件夹名改为 `CodeHighlighter`；

第 3 步：登录管理后台，激活插件；

第 4 步：设置：选择主题风格，是否显示行号等。

**代码写法**

```
\`\`\`javascript(语言类型必填)
// codes go here
\`\`\`
```

**高亮效果图**

![代码高亮.png][3]

## 重要说明

### 可设置项

**1. 选择高亮主题风格** (官方提供的 8 种风格切换)

- coy.css
- dark.css
- default.css
- funky.css
- okaikia.css (默认选中，因为比较顺眼)
- solarized-light.css
- tomorrow-night.css
- twilight.css

**2. 是否在代码左侧显示行号** (默认开启)

### 在插件中不方便实现的设置项

由于 `prismjs` 与 `highlightjs` 的插件扩展机制不同，所以本插件的有些扩展项是无法设置的。

本插件支持常见的一些语言高亮。您可以打开以下链接查看详情：

[http://prismjs.com/download.html#themes=prism-okaidia&languages=markup+css+clike+javascript+apacheconf+c+aspnet+bash+cpp+csharp+coffeescript+markup-templating+git+java+less+markdown+nginx+php+sql+python+smarty&plugins=line-numbers+toolbar+show-language+copy-to-clipboard][4]

如有需要，请勾选需要支持的语言定制您的 js 和 css 文件，下载好后，分别替换以下文件：

`Typecho 插件目录\CodeHighlighter\static\prism.js`

`Typecho 插件目录\CodeHighlighter\static\styles\改为对应的风格名.css` (如跟您博客样式有冲突，稍作修改此 `css` 即可)

**建议**

插件 `Plugins` 最好至少勾选以下 4 项：

- Line Numbers (在代码左侧显示行号)
- Toolbar (代码块右上方工具条)
- Show Language (显示代码是什么语言【依赖: Toolbar】)
- Copy to Clipboard Button (复制代码功能【依赖: Toolbar】)

## 与我联系

作者：Copterfly

主页：[https://www.copterfly.cn/][5]

有问题请留言交流。


  [1]: https://github.com/Copterfly/CodeHighlighter-for-Typecho
  [2]: http://prismjs.com/
  [3]: http://www.copterfly.cn/usr/uploads/2018/05/2713638326.png
  [4]: http://prismjs.com/download.html#themes=prism-okaidia&languages=markup+css+clike+javascript+apacheconf+c+aspnet+bash+cpp+csharp+coffeescript+markup-templating+git+java+less+markdown+nginx+php+sql+python+smarty&plugins=line-numbers+toolbar+show-language+copy-to-clipboard
  [5]: https://www.copterfly.cn/