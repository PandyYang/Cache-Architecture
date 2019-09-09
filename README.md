# Cache-Architecture
高可用技术+架构+解决方案

### 商品详情页的系统架构 -> 缓存架构 -> 高并发 -> 高可用
_小型网站的缓存架构_
![小型网站缓存架构](https://github.com/PandyYang/Cache-Architecture/blob/master/pictures/%E5%B0%8F%E5%9E%8B%E7%BD%91%E7%AB%99%E7%BC%93%E5%AD%98%E6%9E%B6%E6%9E%84.png)
_大型网站的缓存架构_
![大型网站缓存架构](https://github.com/PandyYang/Cache-Architecture/blob/master/pictures/%E5%A4%A7%E5%9E%8B%E7%BD%91%E7%AB%99%E7%BC%93%E5%AD%98%E6%9E%B6%E6%9E%84.png)


html模板发生变更不需进行全量重新渲染,直接将最新的html模板推送到nginx服务器上去就可以了.
在大量请求的情况下数据时直接从nginx本地取的缓存,没有网络请求的开销,没有业务逻辑.渲染到模板中/
