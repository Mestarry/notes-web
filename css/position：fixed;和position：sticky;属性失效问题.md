当元素样式transform属性不为none时，后代元素position:fixed;position:sticky;将失效。

解决方案
不要在transform属性不为none后代元素中使用position:fixed;position:sticky;

解决办法二
通过js动态修改transform属性；