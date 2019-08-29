# jedice


开奖算法验证

1.从萤火钱包资产详情中可以找到转账给GA4HZDTMCUXNXFESLF2A67CXIIS5NDBHWGUQ2L4TPN62AA2U4KXU2BET的转账记录。

2.找到转账的txid 访问链接
https://steexp.com/tx/这里填txid

3.在页面中找到Ledger，点击之后可以看到Hash

或 https://steexp.com/ledger/这里填找到的Ledger

4.找到Hash的后4位，换算成10进制，并按照比例映射到0-99以内

例如后四位是1abc，随机数=parseInt('1abc',16)/praseInt('ffff',16)*99 
