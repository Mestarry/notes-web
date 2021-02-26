### ios低版本客户端，非操作元素点击事件无效

```
<div id="btn">点击</div>
<script>
var btn = document.getElementById('btn');
btn.addEventListener('click', function() {
    alert('点击了按钮');
});
</script>
```
解决办法一
```
// 给元素添加样式属性cursor: pointer;
<style>
#btn{
    cursor: pointer;
}
</style>

<div id="btn">点击</div>
<script>
var btn = document.getElementById('btn');
btn.addEventListener('click', function() {
    alert('点击了按钮');
});
</script>
```

解决办法二
```
// 在元素上直接绑定事件;
<div id="btn" onclick="onClick()">点击</div>
<script>
function onClick() {
    alert('点击了按钮');
};
</script>
```