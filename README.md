# 监听切换浏览器标签的事件
```javascript
var browserHidden = document.hidden ? 'hidden' : document.webkithidden ? 'webkithidden' : document.mozhidden ? 'mozhidden' : null;
var visibChange = 'visibilitychange' || 'webkitvisiblitychange' || 'mozvisibilitychange';
document.addEventListener(visibChange, function() {
  if(browserHidden) {
    // 切换到其他标签
  }else {
    // 切换回本标签
  }
});
