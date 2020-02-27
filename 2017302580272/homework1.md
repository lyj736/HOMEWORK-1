## 分布式计算与网络第一次作业

### 1. ping 另一台计算机
思路：使用命令行ping维护*www.baidu.com*的服务器，结果如下：
<br/><br/>
![avatar](/static/ping.png)
<br/><br/>
分析：所返回的TTL是该字段指定IP包被路由器丢弃之前允许通过的最大网段数量。
### 2. tracert一个服务器
思路：tracert命令用来显示数据包到达目标主机所经过的路由器，并显示到达每个节点的时间, 使用命令行tracert *ip 47.106.106.107*，此ip为本人一服务器，结果如下：
<br/><br/>
![avatar](/static/tracert.png)
<br/><br/>
分析：可以发现有许多请求超时的情况，出现这种情况可能因为那一跳禁PING或者那一跳不对TTL超时做响应处理。
