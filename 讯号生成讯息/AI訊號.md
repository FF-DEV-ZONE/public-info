# AI Signal

AI Signal (ID3) URL(DEBUG):
> http://192.168.25.201:3051/data/agg/id3a

AI Signal (ID3) URL(TEST):
> http://192.168.25.201:3100/data/agg/id3a

AI Signal (ID3) URL(LIVE):
> http://192.168.25.240:3020/data/agg/id3a

DESC:
```
A: 'time'           // 時間
B: 'hsiClose'       // HSI CLOSE
C: 'indUpList'      // 溢放量的板塊
D: 'indDnList'      // 折放量的板塊
E: 'indABList'      // 主买的板塊
F: 'indASList'      // 主卖的板塊
G: 'isHsiSurge'     // 放量 (6, 7, 8 級的放量)
H: 'extUpToDnList'  // 由升轉跌的產品
I: 'extDnToUpList'  // 由跌轉升的產品
J: 'extKeepUpList'  // 持續升的產品
K: 'extKeepDnList'  // 持續跌的產品
L: 'stockVolPer'    // 前幾天對比的量百分比
M: 'buyList',       // 主買的指數
N: 'sellList',      // 主賣的指數
O: 'upResisList',   // 向上阻力的指數
P: 'dnResisList',   // 向下阻力的指數
Q: 'isMktCapLargeDiff' // 大小盘是否有大差異
R: 'mktCapD7SurgeList' // 大小盘有大差異且放量的SYMBOL
```


