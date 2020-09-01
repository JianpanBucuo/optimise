### 2-1 为什么进行web性能优化

1. 内容越来越多
2. 功能越来越强大
3. 页面越来越漂亮

- 速度会受到影响
三秒加载导致 53%跳出率
1. 了解性能指标，多快才算快
2. 利用测量工具和API
3. 优化


### 2-2 性能指标
## Network
chrome network setting 除了group byframe

F12 network 可以看 总请求数/总资源量/DOMContentLoaded？

瀑布图

TTFB 是 Time to First Byte 
浏览器发出请求到 浏览器开始收到服务器响应数据的时间
1. 服务器响应速度（查询数据库/数据组织和处理）
Content Download 代表下载的时间
2. 下载的时间越长/后续的资源阻塞的时间越长

蓝线： dom加载完成的时间
红线： 所有资源加载完成时间

## lighthouse
<!-- https://www.crx4chrome.com/crx/180377/ -->
网络加载的性能
### First Contentful Paint 
First Contentful Paint marks the time at which the first text or image is painted

### Speed Index 
标准4s
Speed index shows how quickly the contents of a page are visibly populated

交互体验 （目的： 及时给用户反馈）
1. 交互响应
2. 帧数（向下滚动时页面卡顿/动画卡）
ctrl + shift + p 
show frames per second
3. 异步请求 一秒