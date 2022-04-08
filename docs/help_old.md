# etsuko 食用说明

> 更新时间：2022-02-25 15:54


> 文件阅读说明
> - `<XXX>` XXX为必填内容
> - `[XXX]` XXX为选填内容

## [etsuko tg bot](https://t.me/nicoetsukobot)  (telegram机器人)

> 阅读说明
>
> - 命令与要填写的内容中间请用至少一个空格隔开
> - 🇷 —— 支持通过指令回复内容
> - 🇵 —— 仅支持私聊
> - 🇬 —— 仅支持群聊
> - ⚠︎——测试类型的接口（详情请看参与测试部分的说明）

### 机器人地址

https://t.me/nicoetsukobot

#### 检测节点

##### /check <订阅链接或节点>

> ⚠︎🇷 检测订阅或节点的可用性

例如：
`/check https://v2ray.neocities.org/v2ray.txt`

##### /speed <订阅链接或节点>

> ⚠︎检测节点的速度

例如：

`/speed https://v2ray.neocities.org/v2ray.txt`

##### /check_base <订阅链接或节点>

> ⚠︎🇷 获取基础版的测试报告，图片格式输出（PNG）

例如：
`/check_base https://v2ray.neocities.org/v2ray.txt`

##### /check_full <订阅链接或节点>

> ⚠︎🇷 获取详细版的测试报告，图片格式（PNG）

例如：
`/check_full https://v2ray.neocities.org/v2ray.txt`

##### /check_base_xls <订阅链接或节点>

> ⚠︎🇷 获取基础版的测试报告，表格格式（XLSX）

例如：
`/check_base_xls https://v2ray.neocities.org/v2ray.txt`

##### /check_full_xls <订阅链接或节点>

> ⚠︎🇷 获取详细版的测试报告，表格格式（XLSX）

例如：
`/check_full_xls https://v2ray.neocities.org/v2ray.txt`

#### 自动检测预警

##### /check_task_add <订阅链接>

> ⚠︎将订阅链接添加至定时检测中，默认检测间隔60分钟，订阅会缓存3个小时

例如：
`/check_task_add https://v2ray.neocities.org/v2ray.txt`

##### /check_task_del <检测编号>

> ⚠︎将已经在任务内的检测任务永久移除（无法恢复）

例如：
`/check_task_del https://v2ray.neocities.org/v2ray.txt`

##### /check_task

> ⚠︎编辑当前任务配置，支持：
> - 检测间隔
> - 存活率报警阈值
> - 刷新缓存
> - 移除配置

#### 杂项

##### /status

> ⚠︎获取当前的运行状态

##### /suggest <建议内容>

> 提供建议、bug等

例如：
`/suggest 快点修bug ！！！`

##### /help

> 查看帮助

## ⚠︎参与测试

> - 可以尝试一些新的功能
> - 可以提出自己的奇思妙想说不定就可以变成机器人的功能

### tg机器人

#### 注意事项

- 参与测试仅仅代表参与某一个版本、某一个功能，当测试结束后，会自动清除，如果想参与后续的测试，需要在下个版本的时候重新报名

#### 个人参与

- 在私聊中给机器人发送 `/uid` 的指令
- 将上一步机器人返回的结果告知给开发者，让开发者手动添加到测试中

#### 群聊参与

- 在群聊中给机器人发送 `/gid` 的指令，请确保你有管理员权限
- 将上一步机器人返回的结果告知给开发者，让开发者手动添加到测试中
- 如果不想在自己的群聊中测试的话，可以进入 https://t.me/+X2v1oflF60g1YWE9 进行测试和bug反馈
