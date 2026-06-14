# 个人中心

个人中心用于查看和管理当前用户账户。它将整体资产、复制交易账户、主钱包交易账户和个人资料集中到一个页面中。

## 页面入口

| 页面 | 地址 | 说明 |
| --- | --- | --- |
| Overview | `/profile` | 查看账户整体表现。 |
| Copies | `/profile?tab=copies` | 查看复制交易账户。 |
| Perpetuals | `/profile?tab=perpetuals` | 查看主钱包统一交易账户。 |

{% hint style="info" %}
个人中心需要登录后访问。未登录用户会被引导至 Smart Money 页面。
{% endhint %}

## Overview

Overview 是账户总览页面，用于查看主钱包和复制交易账户合并后的整体表现。

主要用于确认：

- 当前账户估算总值
- 7 日 PnL
- 资产分布
- 充值与提现记录
- 个人资料入口

## Copies

Copies 是复制交易账户页面，只展示复制交易相关数据，不与用户自己的主钱包交易混在一起。

用户可以查看：

- Copy Trading Equity
- 7D PNL
- Available Margin
- PnL
- Unrealized PnL
- 活跃复制规则
- 复制交易历史

常见操作：

- 创建复制交易
- 停止全部复制交易
- 查看历史复制记录

{% hint style="warning" %}
复制交易状态由后端异步处理。创建、关闭或调整策略后，数据可能需要短时间同步。
{% endhint %}

## Perpetuals

Perpetuals 展示用户自己的主钱包统一交易账户。

主要内容包括：

- 当前持仓
- 现货资产
- 成交历史
- 当前挂单
- 资金费率历史
- 历史订单

## My Profile

点击 **My Profile** 可以进入个人资料设置。

可管理内容包括：

| 项目 | 说明 |
| --- | --- |
| Avatar | 上传或更新头像。 |
| Display name | 修改展示名称。 |
| UID | 复制 SeaBond UID。 |
| VIP level | 查看当前 VIP 等级。 |
| Description | 添加或修改个人简介。 |
| Fees | 查看当前手续费信息。 |

## 数据口径

| 区域 | 数据范围 |
| --- | --- |
| Overview | 主钱包 + 复制交易子钱包。 |
| Copies | 仅复制交易子钱包。 |
| Perpetuals | 仅主钱包统一交易账户。 |

这种区分可以帮助用户判断：收益来自自己直接交易，还是来自复制交易账户。

