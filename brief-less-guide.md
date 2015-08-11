### 0 前言

我们的目标是：不管有多少人共同参与同一项目，一定要确保每一行代码都像是同一个人编写的。

虽然本文档是针对CSS设计的，但是在使用各种CSS的预编译器(如less、sass、stylus等)时，适用的部分也应尽量遵循本文档的约定。

#### 1. [强制] 当一个 rule 包含多个 selector 时，每个选择器声明必须独占一行。
#### 2. [强制] 属性定义必须另起一行。
#### 3. [建议] 选择器的嵌套层级应不大于 3 级，位置靠后的限定条件应尽可能精确。
#### 4. [建议] 代码组织

同一 rule set 下的属性在书写时，应按功能进行分组，并以 Formatting Model（布局方式、位置） > Box Model（尺寸） > Typographic（文本相关） > Visual（视觉效果） 的顺序书写，以提高代码的可读性。

解释：

Formatting Model 相关属性包括：position / top / right / bottom / left / float / display / overflow 等
Box Model 相关属性包括：border / margin / padding / width / height 等
Typographic 相关属性包括：font / line-height / text-align / word-wrap 等
Visual 相关属性包括：background / color / transition / list-style 等
另外，如果包含 content 属性，应放在最前面。排序的原则是：影响优先级越大，越前面。

