---
title: Markdown示例
published: 2023-10-01
description: 一个简单的Markdown博客文章示例。
tags: [Markdown, 博客]
category: 示例
draft: true
---

## 目录

# 一个 h1 标题

段落之间通过一个空行分隔。

第二段。_斜体_，**粗体**，和`等宽字体`。项目列表看起来像这样：

- 这个
- 那个
- 另一个

注意，不考虑星号的话，实际文本内容是从第 4 列开始的。

> 块引用是这样写的。
>
> 如果需要，它们可以跨越多个段落。

使用 3 个短横线来表示破折号。使用 2 个短横线来表示范围（例如，“都在章节 12--14 中”）。三个点...将被转换为省略号。支持 Unicode。☺

## 一个 h2 标题

这里是一个编号列表：

1. 第一个项目
2. 第二个项目
3. 第三个项目

再次注意，实际文本是从第 4 列开始的（从左边起 4 个字符）。这里有一个代码示例：

    # 让我重复一遍...
    for i in 1 .. 10 { do-something(i) }

如您所猜测的，缩进 4 个空格。顺便说一下，如果您愿意，可以使用分隔块而不是缩进块：

```
define foobar() {
    print "Welcome to flavor country!";
}
```

（这使得复制和粘贴更容易）。您可以选择性地为 Pandoc 标记分隔块以进行语法高亮：

```python
import time
# 快速，数到十！
for i in range(10):
    # （但不要太快）
    time.sleep(0.5)
    print i
```

### 一个 h3 标题

现在是一个嵌套列表：

1.  首先，获取这些材料：

    - 胡萝卜
    - 芹菜
    - 扁豆

2.  煮一些水。

3.  把所有东西都倒进锅里，然后按照这个算法操作：

        找到木勺
        揭开锅盖
        搅拌
        盖上锅盖
        在锅把上不稳定地平衡木勺
        等待10分钟
        转到第一步（或者完成后关闭炉子）

    不要碰到木勺，否则它会掉下来。

再次注意，文本总是对齐 4 个空格的缩进（包括上面继续第 3 点的最后一行）。

这里有一个链接到[一个网站](http://foo.bar)，到[本地文档](/posts/video/)，以及到当前文档中的[一个 h2 标题](#一个h2标题)。这里有一个脚注[^1]。

[^1]: 脚注文本放在这里。

表格可以像这样：

| 尺寸 | 材料   | 颜色 |
| ---- | ------ | ---- |
| 9    | 皮革   | 棕色 |
| 10   | 麻布料 | 原色 |
| 11   | 玻璃   | 透明 |

表：鞋子，它们的尺寸，以及它们的材料

（以上是表格的标题。）Pandoc 还支持多行表格：

| 关键词 | 文本                                             |
| ------ | ------------------------------------------------ |
| 红色   | 日落，苹果，以及其他红色或红褐色的东西。         |
| 绿色   | 叶子，草地，青蛙，以及其他不容易成为绿色的东西。 |

下面是一个水平线。

---

这里是一个定义列表：

苹果
: 适合做苹果酱。

橙子
: 柑橘类！

番茄
: 番茄中没有“e”。

再次注意，文本缩进 4 个空格。（在每个术语/定义对之间放一个空行可以使内容分布得更开。）

这里是一个“行块”：

| Line one
| Line too
| Line tree

图片可以这样指定：

![示例图片](./guide/cover.jpeg '一个杰出的图片')

行内数学方程式可以这样输入：$\omega = \frac{d\phi}{dt}$。显示数学应该单独占一行，并用双美元符号包围：

$$I = \int \rho R^{2} dV$$

请注意，您可以使用反斜杠转义任何您希望以文本形式显示的标点符号，例如：\`foo\`，\*bar\*，等等。
