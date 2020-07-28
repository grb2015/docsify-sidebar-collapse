# docsify-sidebar-collapse

![](https://img.shields.io/npm/v/docsify-sidebar-collapse.svg)
![](https://img.shields.io/github/license/iPeng6/docsify-sidebar-collapse.svg)

support docsify sidebar collapsed default

## Preview

![](assets/show.gif)

## Usage

Firstly, make sure that the [loadSidebar](https://docsify.js.org/#/configuration?id=loadsidebar) config is enabled，and the Markdown file `_sidebar.md` is provided in the root directory.

Then insert script into document just like the [official plugins](https://docsify.js.org/#/plugins)'s usage

```html
 <script>
    window.$docsify = {
      loadSidebar: true,
      alias: {
        '/.*/_sidebar.md': '/_sidebar.md',
      },
      subMaxLevel: 3,
      ...
    }
  </script>
  <script src="//unpkg.com/docsify/lib/docsify.min.js"></script>

  <!-- plugins -->
  <script src="//unpkg.com/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js">
```


 ## grb_docsify_practice/docs 是用![](https://docsify.js.org/#/zh-cn/quickstart)写的一个demo，用于测试插件。

 ## bug1: 目录点击后无法折叠
   bug演示：https://github.com/grb2015/docsify-sidebar-collapse/blob/master/assets/grb_bug1.mp4
   bug描述：点击"1.1二级标题"后，子目录被展开，是正确的。再点击一次后，子目录应该被折叠。
   bug节点： [add] 上传bug1.mp4 20200720 
   期望结果：点击"1.1二级标题"后，子目录被展开，是正确的。再点击一次后，子目录应该被折叠。
   
   

