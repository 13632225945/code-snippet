# 监听切换浏览器标签的事件
```javascript
var browserHidden = 'hidden' in document ? 'hidden' : 'webkithidden' in document ? 'webkithidden' : 'mozhidden' in document ? 'mozhidden' : null;
var visibChange = 'visibilitychange' || 'webkitvisiblitychange' || 'mozvisibilitychange';
document.addEventListener(visibChange, function() {
  if(browserHidden) {
    // 切换到其他标签
  }else {
    // 切换回本标签
  }
});
