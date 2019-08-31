# jedice

# 开奖算法验证v2

1. 从萤火钱包资产详情中可以找到转账给*GA4HZDTMCUXNXFESLF2A67CXIIS5NDBHWGUQ2L4TPN62AA2U4KXU2BET*的转账记录。

2. 找到转账的txid访问链接  
   https://steexp.com/tx/这里填txid

3. 在页面中找到Ledger，点击之后可以看到Hash  
   或 https://steexp.com/ledger/这里填找到的Ledger

4. Hash长度是64，前40位做为第一个随机数种子s1，后24位为第二个随机数种子s2，将两个种子分别转换成16进制数组。  
   进行以下计算得出开奖结果

``` 
result = (uint64(s1[0]) + uint64(s2[1]) + uint64(s1[2]) 
         + uint64(s2[3]) + uint64(s1[4]) + uint64(s2[5]) 
         + uint64(s1[6]) + uint64(s2[7]))%100 
```


