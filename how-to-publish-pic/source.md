# 如何使用github作为图床，实现多平台发布博客文章

### 1. 问题描述

写的文章图片比较多，发布多个平台要重复编辑上传好多次，每个平台都会单独增加水印，所以需要找一个地方放原图，然后各个平台自动转存图片。


### 2.解决方案

可以使用 github（或者gitee）作为图床，存储原始图片，然后使用 markdown 编辑工具编辑文章，文章中使用图片的原始地址，写好后粘贴到各个平台会自动进行转存。

### 3.方法举例

1. 在 github （或者gitee）中创建一个新的仓库，专门用来存放图片
2. 将创建的项目克隆到本地。
3. 将需要用到的图片推送到仓库中。
4. 在仓库中找到图片路径，将路径中的 blob 替换成 raw，按回车后，获取图片的实际存储路径，如下图所示

![原路径](https://raw.githubusercontent.com/liu-shichao/blog-pic/main/how-to-publish-pic/1.png)

![修改成raw](https://raw.githubusercontent.com/liu-shichao/blog-pic/main/how-to-publish-pic/2.png)

![按回车后获取的真实路径](https://raw.githubusercontent.com/liu-shichao/blog-pic/main/how-to-publish-pic/3.png)


5. 使用 markdown工具编辑文档，粘贴到各个平台，发布。

### 4.参考示例

这篇文档的 markdown 源文件及图片都放在下边这个仓库里了，可以参考查看。
https://github.com/liu-shichao/blog-pic/tree/main/how-to-publish-pic
其中的 source.md 是这篇文档的源文件。
