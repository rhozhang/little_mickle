# perpetuity

tag: finance

perpetual bond

## 国内首单永续债

[金融时报记者孙璐璐, 2019-01-28, 中行永续债发行获超额认购, 业界盼监管细则进一步明确][1]

2019-01-25, 中国银行在全国银行间债券市场发行首单银行永续债，拉开了我国银行业通过永续债补充其他一级资本的大幕。
该债券的外部评级为 AAA，发行规模 400 亿元，票面利率 4.5%，预计可以提高中行一级资本充足率 0.3 个百分点

中行永续债发行获得了市场高度关注，共有约 140 家机构参与认购，还成功吸引数家境外机构参与投资，
一次性完成发行上限目标，实现两倍以上超额认购；路演时投资者反馈的票面利率区间在 4.5%～5.2%，市场普遍预期在 4.7%，
但最终票面利率位于区间下端

2018-12-25，国务院金融稳定发展委员会办公室召开专题会议，指出要尽快启动永续债（包括无固定期限资本债券）的发行，来解决商业银行
多渠道补充资本的有关问题。自此，永续债发行进入快车道

哪类投资者青睐永续债? 申万宏源证券首席银行业分析师马鲲鹏也表示，从海外经验看，预计以险资、银行资管为代表的追求长期、稳定、绝对收益的机构投资者对永续债的
偏好度较高. 永续债有利于拉长资产久期、优化资产负债匹配、分散投资组合风险

主要问题

- 流动性。与一般利率品种和普通金融债相比，银行资本债券的流动性相对缺乏，而非银机构投资者普遍比较关注债券的流动性价值，
特别是其作为抵押品融资的能力。
- 银行互持问题。根据《商业银行资本管理办法（试行）》，商业银行之间通过协议相互持有的各级资本工具，或银保监会认定为
虚增资本的各级资本投资，应从相应监管资本中对应扣除。为了防止银行虚增资本，对于银行互持或是银行间接购买本行资本补充
工具的行为，都应从相应的监管资本中扣除。然而，现实中，银行通过表外资金绕道委外投资本行资本工具的情况较多，这些资金
本质上是银行的负债或是客户委托给银行进行理财的资金，但用来补充本行资本且未有相应的资本扣除，有虚假注资的嫌疑。

2019-02-19，人行 (PBoC) 副行长潘功胜在记者会上表示，中行的永续债受到市场投资者的广泛欢迎，其他银行正“积极筹备”发行永续债, 
以便在中国经济预期将会出现的放缓之前补充这些机构的资本

“部分银行面临着资本约束，”潘功胜表示，“加之监管标准趋严, 一些影子银行业务回表等因素影响，商业银行资本补充面临更高的要求。”

## UK consols

[wikipedia][2]: UK government bonds (called consols) were undated as well as irredeemable except by act of Parliament. 
As in war bonds, they were paid fixed coupons, and traded actively in the bond market until the government 
redeemed them in 2015

[britannica][3]: Consol, British government security without a maturity date. The name is a contraction for 
**Consolidated Annuities**, a form of British government stock that originated in 1751. The first issue of consols 
carried an interest rate of 3 percent (reduced to 2.75 percent in 1888 and to 2.5 percent in 1902). 
Between the years 1926 and 1932, 4 percent consols were issued. Although consols formed the larger part of 
Britain’s funded debt before World War I, in 1961 they accounted for less than 3 percent of the total national 
debt because of the vast expansion of other forms of government debt during the two world wars. 
The 4 percent consols became redeemable on three months’ notice after Feb. 1, 1957

The 2.5 percent consols are in practice irredeemable by the government, and their price tends to vary 
with the bank rate

## Historical data of UK consols

[FRED][4]: Consol (Long-term bond) yields in the United Kingdom

- symbol: LTCYUK
- frequency: quarterly
- period: 1753-07-01 --- 2016-10-01

```r
library("quantmod")
getSymbols("LTCYUK", src = "FRED")
```

[1]: http://www.cs.com.cn/jg/04/201901/t20190128_5919832.html
[2]: https://en.wikipedia.org/wiki/Perpetuity
[3]: https://www.britannica.com/topic/consol-economics
[4]: https://fred.stlouisfed.org/series/LTCYUK
