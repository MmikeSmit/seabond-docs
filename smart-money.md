# 聪明钱发现

聪明钱是你在 SeaBond 里发现交易钱包的地方。它会把不同钱包的表现、交易活跃度和风险特征集中展示，方便你快速找到可以进一步查看的钱包。

用户通常会在这里完成第一步判断：哪些钱包表现突出，哪些钱包需要继续看详情，哪些钱包可以加入收藏后持续观察。

## 先看钱包表现

聪明钱列表的核心不是单独看收益，而是把收益、回撤、交易次数、账户规模和近期表现放在一起看。

一个值得继续查看的钱包，通常需要同时满足几个条件：

- 有足够的交易样本
- 收益来源相对清晰
- 回撤在可接受范围内
- 近期表现和长期表现没有明显冲突
- 当前持仓没有明显失控

这样你可以更快判断：这个钱包只是短期表现突出，还是有继续查看的价值。

## 钱包画像标签

钱包卡片头像旁边会展示一组系统标签，用来快速概括这个钱包的交易特征。它们不是用户手动添加的收藏标签，而是根据钱包数据生成的画像。

常见标签包括：

| 标签类型 | 示例 | 含义 |
| --- | --- | --- |
| 账户规模 | <img src="assets/smart-money/whale.svg" alt="鲸鱼" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 鲸鱼、<img src="assets/smart-money/shark.svg" alt="鲨鱼" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 鲨鱼、<img src="assets/smart-money/dolphin.svg" alt="海豚" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 海豚、<img src="assets/smart-money/fish.svg" alt="小鱼" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 小鱼 | 按当前持仓规模区分钱包体量。 |
| 币种偏好 | <img src="assets/smart-money/majors.svg" alt="主流币" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 主流币、<img src="assets/smart-money/alts.svg" alt="山寨币" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 山寨币、<img src="assets/smart-money/tradfi.svg" alt="TradFi" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> TradFi、<img src="assets/smart-money/mixed.svg" alt="综合" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 综合 | 判断钱包主要交易哪些类型的标的。 |
| 方向偏好 | <img src="assets/smart-money/long-biased.svg" alt="偏多" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 偏多、<img src="assets/smart-money/short-biased.svg" alt="偏空" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 偏空、<img src="assets/smart-money/hybrid.svg" alt="均衡型" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 均衡型 | 判断钱包更常做多、做空，还是多空相对均衡。 |
| 交易周期 | <img src="assets/smart-money/trend.svg" alt="超短线" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 超短线、<img src="assets/smart-money/short-term.svg" alt="短线" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 短线、<img src="assets/smart-money/high-freq.svg" alt="中长线" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 中长线 | 判断钱包更偏短频交易，还是更长周期持仓。 |
| 表现标记 | <img src="assets/smart-money/on-fire.svg" alt="胜率狂人" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 胜率狂人、<img src="assets/smart-money/shield.svg" alt="稳定增值" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 稳定增值、<img src="assets/smart-money/lightning.svg" alt="赚钱机器" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 赚钱机器 | 对胜率、稳定性或交易活跃度表现较突出的钱包做提示。 |

例如截图里的 **均衡型 / 偏多 / 短线**，表示这个钱包在画像上多空分布相对均衡、近期方向更偏多，交易节奏偏短线。用户可以先通过这些标签判断它是否符合自己的跟单偏好，再进入详情页看持仓和历史交易。

### 账户规模怎么判断

账户规模按当前持仓金额划分：

| 标签 | 判断标准 |
| --- | --- |
| <img src="assets/smart-money/whale.svg" alt="鲸鱼" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 鲸鱼 | 持仓大于 100 万 USDC |
| <img src="assets/smart-money/shark.svg" alt="鲨鱼" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 鲨鱼 | 持仓 10 万到 100 万 USDC |
| <img src="assets/smart-money/dolphin.svg" alt="海豚" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 海豚 | 持仓 5 万到 10 万 USDC |
| <img src="assets/smart-money/fish.svg" alt="小鱼" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 小鱼 | 持仓 1 万到 5 万 USDC |

这个标签主要用来判断钱包体量。体量越大，通常越能代表真实资金行为；体量较小的钱包，收益率可能更容易被少数交易放大。

### 表现标记怎么判断

表现标记用于提示近期交易表现比较突出的账户：

| 标签 | 判断标准 |
| --- | --- |
| <img src="assets/smart-money/on-fire.svg" alt="胜率狂人" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 胜率狂人 | 胜率大于 80%，且 30 日开单数大于 60 |
| <img src="assets/smart-money/shield.svg" alt="稳定增值" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 稳定增值 | 半年以上稳定盈利，且 30 日开单数大于 30 |
| <img src="assets/smart-money/lightning.svg" alt="赚钱机器" width="18" style="display:inline-block;vertical-align:middle;margin-right:4px;" /> 赚钱机器 | 胜率大于 60%，且 30 日开单数大于 300 |

这些标记只说明钱包符合对应的数据条件，不代表后续一定会继续盈利。判断是否跟随时，还需要结合当前持仓、回撤、杠杆和交易币种一起看。

## 怎么筛第一批候选钱包

你可以先用比较硬的条件缩小范围。

### 看账户规模

账户太小的钱包容易出现数据失真。比如一个小账户刚好抓住一笔大行情，收益率会非常好看，但不一定代表策略稳定。

### 看收益来源

总盈亏适合做第一眼判断，但还需要看收益是不是来自持续交易，还是只靠一两笔大单。

如果一个钱包大部分收益都来自单笔交易，可以把它加入收藏，后续结合更多交易记录再判断。

### 看交易次数

交易次数太少，样本不够；交易次数太多，可能是高频或短线策略。高频策略跟随时更容易受滑点、延迟和手续费影响。

### 看回撤

回撤比收益更重要。一个钱包如果赚得多但回撤也很深，你跟单时未必能扛住中间那段亏损。

### 看近期和长期是否一致

近期突然爆发的钱包要谨慎。更值得观察的是：近期表现不错，同时长期也没有明显失控。

## 看到一个钱包后怎么判断

可以按这个顺序看：

1. 它是不是长期稳定，而不是短期暴利？
2. 它有没有明显重仓或高杠杆习惯？
3. 它主要交易哪些币？你是否能接受这些币的波动？
4. 它亏损时会不会继续加仓？
5. 它平仓是否有规律？
6. 它现在的持仓是否已经不适合追进去？

{% hint style="info" %}
聪明钱列表适合做第一轮筛选。进入钱包详情页后，可以继续查看持仓、历史交易和更完整的风险数据。
{% endhint %}

## 推荐的工作流

1. 用筛选条件找出 10 到 20 个候选钱包。
2. 打开详情页，排除明显高风险的钱包。
3. 把剩下的钱包加入收藏。
4. 给每个钱包打标签，记录你为什么关注它。
5. 根据后续表现，选择继续观察或创建跟单。

## 什么时候应该排除一个钱包

如果出现下面情况，建议直接排除或只放入观察：

- 账户规模过小但收益率极高
- 收益曲线主要靠单笔暴利拉升
- 当前持仓已经大幅浮盈
- 经常满仓或高杠杆交易
- 回撤明显超过你的承受范围
- 最近交易风格和过去完全不同

{% hint style="warning" %}
SeaBond 可以帮你更快发现钱包，但不能替你判断风险。跟单前请先确认这个钱包的交易方式是否真的适合你。
{% endhint %}
