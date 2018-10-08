不要把content内容在CSS里写死，使用attr表达式来从页面元素中动态的获取内容
content: attr(data-text); /* 属性名称上不要加引号！ */

css3为了区分伪类和伪元素，伪元素采用双冒号写法
常见伪类——:hover,:link,:active,:target,:not(),:focus。
常见伪元素——::first-letter,::first-line,::before,::after,::selection。

::before和::after下特有的content，用于在css渲染中向元素逻辑上的头部或尾部添加内容。
这些添加不会出现在DOM中，不会改变文档内容，不可复制，仅仅是在css渲染层加入。
所以不要用:before或:after展示有实际意义的内容，尽量使用它们显示修饰性内容
