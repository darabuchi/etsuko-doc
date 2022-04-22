# etsuko 食用说明

> 文件阅读说明
> - `<XXX>` XXX为必填内容
> - `[XXX]` XXX为选填内容

## [etsuko tg bot](https://t.me/nicoetsukobot)  (telegram机器人)
> 阅读说明
> - 如无特殊说明，仅支持 `clash` 订阅
> - 命令与要填写的内容中间请用至少一个空格隔开
> - 🇷 —— 支持通过指令回复内容
> - 🇵 —— 仅支持私聊
> - 🇬 —— 仅支持群聊
> - ⚠︎ ——测试类型的接口

### /check <订阅链接或节点>

> 检测订阅或节点的可用性
> 支持测试结果导出 图片(png)和表格(Excel)

例如：
`/check https://v2ray.neocities.org/clash.xml`

### /speed <订阅链接或节点>

> 检测订阅或节点的速度
> 支持测试结果导出 图片(png)和表格(Excel)

例如：
`/speed https://v2ray.neocities.org/clash.xml`

### /check_info <订阅链接或节点>

> 检测订阅或节点的基本信息
>   - 入口信息
>   - 出口信息
> 如果节点本身不可用，则获取不到信息
> 支持测试结果导出 图片(png)和表格(Excel)

例如：
`/check_info https://v2ray.neocities.org/clash.xml`

### /check_unlock <订阅链接或节点>

> 检测订阅或节点的解锁信息，支持：
>   - Netflix
>   - Youtube
>   - Disney+
> 如果节点本身不可用，则获取不到信息
> 支持测试结果导出 图片(png)和表格(Excel)

例如：
`/check_unlock https://v2ray.neocities.org/clash.xml`

### /check_full <订阅链接或节点>

> 检测订阅或节点的全部信息，为了不保证稳定性，速度较慢

例如：
`/check_full https://v2ray.neocities.org/clash.xml`

## 当前支持的节点协议

### clash协议

- trojan
- vmess
- ss
- ssr
- socket
- http
- vless

### v2ray协议

- trojan
- vmess
- ss
- ssr
- vless

## 测试的相关说明

### 可用性测试

- 可用性测试是测试节点是否可以正常访问Google，展示的延时是指加载完Google的页面的耗时
- 如果加载时间超过了5秒则认为节点不可用

### 速度测试

- 速度测试对齐 v2rayN 是测速结果，结果可能会存在上下浮动的情况（如果想要完全一致理论上只有和机器人部署的所在网络一致才可以）
- 如果节点过慢会自动断开链接终止测速以释放资源（并不代表无速度）

### TcpPing测试

- TcpPing测试是测试节点是否可以正常访问节点的域名、IP、端口等，不代表节点是否可用
- 如果连接时间超过了1秒则认为连接失败
- 测试结果主要判断是否是节点的入口服务器出现了故障
- 低延时也不代表最终访问延时低，也不代表速度快，很多机场会使用国内中转的方案，这种方案最容易造成低Ping延时，高访问延时，而速度和延时没有太大关系

### UdpPing测试

- UdpPing测试是测试节点是否支持UDP访问
- 如果连接时间超过了1秒则认为连接失败
- 低延时也不代表最终访问延时低，也不代表速度快，很多机场会使用国内中转的方案，这种方案最容易造成低Ping延时，高访问延时，而速度和延时没有太大关系
