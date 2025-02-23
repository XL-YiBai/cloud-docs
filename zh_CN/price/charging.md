
# 计费说明


## Serverless

### 计费项目

EMQX Cloud Serverless 按照部署实际使用量计费，连接实际产生的**连接分钟数**以及消息产生的**流量**进行计费。用户每个月开始都会获得一定的免费额度，且都会优先使用免费额度。当某一项免费额度用完之后，此项就会进入计费。


### 计费方式
EMQX Cloud 累积**24小时**的连接分钟数以及流量，在每天的0点进行结算，计入小时账单并从余额中扣费。您可以前往 [账单页面](<https://cloud.emqx.com/console/billing/overview>) 查看详细扣费信息。

::: tip Tip
假设一个用户24小时之内，有10个小时客户端连接为120，有10个小时客户端连接为20，有4个小时客户端连接为0，则当天的连接分钟数为：120 * 60 * 10 + 20 * 60 * 10 + 0 = 84,000， 如果在免费额度内，则当天的连接费为0；如果免费额度已经用完，则当天的连接费用为 84,000 / 1,000,000 * 8 = 0.672, 四舍五入的价格为 ¥ 0.67。
流量的计算方式同连接。
:::


### 欠费说明
免费额度用完之后，按照使用情况进行计费并且在余额中扣费。当帐户的余额小于0之后，部署将停止。为了不对您的业务造成影响，请保持余额充足。部署由于欠费停止之后，如需要再次启动使用，需补充所欠费额度。

由于专有版按时计费部署也是消耗帐户余额，如果帐户下既有 Serverless 部署也有专有版按时计费部署，如果帐户余额处于欠费状态下，则会影响所有部署的使用。


## 专有版


### 计费项目

EMQX Cloud 专有版按产品版本、实例规格与消息传输网络流量计费。不限制消息条数，API调用次数与数据集成的使用。您可根据您的业务情况选择对应的产品和规格，当业务扩张时也确保成本仍然清晰可控。

EMQX Cloud 专有版的计费由两部分组成：

| 项目     | 描述                                                         |
| -------- | ------------------------------------------------------------ |
| 基础费用 | 根据部署时所选择的产品版本和实例规格（最大连接数、消息 TPS）对应的小时单价计算出的实例基础费用。实际使用中该部分费用仅跟时长相关，不会因为用量（连接数、消息 TPS）的变动而变动。 |
| 流量使用 | 各实例规格均包含了一定量的免费流量。赠送的流量当月有效，如有剩余月底自动清空。当设备通信超出赠送的流量后超出部分将收取流量费用。 |

创建部署时 EMQX Cloud 会根据您的实例规格选择情况估算使用成本，在正式部署前您可以在确认页面查看到预估价格。

::: warning
由于实际使用情况不同，估计成本与实际成本之间可能存在差异。
:::


### 计费方式

**每小时**统计核算一次上小时内专有版部署消费情况（小时账单）并从余额扣费，然后累加到当月消费（月账单），您可以前往 [账单页面](<https://cloud.emqx.com/console/billing/overview>) 查看详细扣费信息。



## 帐户欠费说明

余额不足时 EMQX Cloud 将发余额不足提醒邮件到注册邮箱。当帐户欠费之后，我们在确认之后会停止并删除您的部署实例。在部署删除之前，补足欠费即可保留和重新开启使用。

