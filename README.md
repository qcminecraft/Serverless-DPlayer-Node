# Serverless-DPlayer-PHP

## 这是什么？
使用[腾讯云函数（SCF）](https://url.cn/55F1LtN)PHP 7搭建的无服务器Dplayer弹幕后端

### 和[MoePlayer/DPlayer-node](https://github.com/MoePlayer/DPlayer-node)比有什么不一样吗？

```diff
+ ~~使用PHP v7，PHP才是最好的语言！（划掉~~
+ 本项目无需安装服务器、依赖等，可以直接部署
+ 腾讯云函数有一定免费额度，在请求少的情况下成本几乎为零，无需购买VPS
+ 可以设置敏感词，屏蔽广告等
! 无法100%兼容Dplayer，如无法限制最大弹幕数量
- 高并发下性能不明
```
## 怎么用啊？

### 0x0001
首先，你需要有一个腾讯云账号 ->[点我注册](https://url.cn/5lgcrXW)

### 0x0002
在云函数列表新建一个函数，地域建议广东：支持API网关
![image.png](https://i.loli.net/2020/05/05/E56lYMm7TdjzSWP.png)
选择空白函数
![image.png](https://i.loli.net/2020/05/05/w1LdGBkr74ocyfx.png)
下载一个最新的[Release](https://github.com/qcminecraft/Serverless-DPlayer-PHP/releases)，上传
![image.png](https://i.loli.net/2020/05/05/rFQUCxHuEij6ZT5.png)
在触发管理中添加一个API网关的触发器

### 0x0003
配置danmaku.php中的信息，完成！
Dplayer后端地址形如 https://service-henghenghengaaa-114514.gz.apigw.tencentcs.com/release/danmaku/
