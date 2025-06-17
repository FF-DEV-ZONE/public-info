# AI Signal

AI Signal (ID3) URL(DEBUG):
> http://192.168.25.201:3051/data/agg/id3a

AI Signal (ID3) URL(TEST):
> http://192.168.25.201:3100/data/agg/id3a

AI Signal (ID3) URL(LIVE):
> http://192.168.25.240:3020/data/agg/id3a


### ---legend---

## col-header:
| (index) | Values              | DESC |
| --- | --- | --- |
| A       | 'time'              | 時間         |         
| B       | 'hsiClose'          | HSI CLOSE            |     
| C       | 'indUpList'         | 溢放量的板塊               |   
| D       | 'indDnList'         | 折放量的板塊               |   
| E       | 'indABList'         | 主买的板塊                |    
| F       | 'indASList'         | 主卖的板塊                |    
| G       | 'isHsiSurge'        | 放量 (6, 7, 8 級的放量)    |               
| L       | 'stockVolPer'       | 前幾天對比的量百分比           |       
| M       | 'buyList'           | 主買的指數                |    
| N       | 'sellList'          | 主賣的指數                |    
| O       | 'upResisList'       | 向上阻力的指數              |      
| P       | 'dnResisList'       | 向下阻力的指數              |      
| Q       | 'isMktCapLargeDiff' | 大小盘是否有大差異            |        
| R       | 'mktCapD7SurgeList' | 大小盘有大差異且放量的SYMBOL    |              


### col(C,D,E,F,G):
| (index)    | Values |
| --- | --- |
| IT         | 'A1'   |
| INSURANCE  | 'A2'   |
| BANK       | 'A3'   |
| AUTO       | 'A4'   |
| INTERNET   | 'A5'   |
| HK35       | 'A6'   |
| SECURITIES | 'A7'   |


### col(H,I,J,K):
| (index)                    | Values |
| --- | --- |
| HHLL_TREND:PRECIOUS_METALS | 'B1'   |
| HHLL_TREND:COMMODITIES     | 'B2'   |
| HHLL_TREND:CRYPTO          | 'B3'   |
| HHLL_TREND:CHINA_BONDS     | 'B4'   |
| HHLL_TREND:EURO_BONDS      | 'B5'   |
| HHLL_TREND:US_BONDS        | 'B6'   |
| HHLL_TREND:HANGSENG        | 'B7'   |
| HHLL_TREND:FTSE            | 'B8'   |
| HHLL_TREND:CAC             | 'B9'   |
| HHLL_TREND:SPTRD           | 'B10'  |
| HHLL_TREND:NASDAQ          | 'B11'  |
| HHLL_TREND:RUSSELL         | 'B12'  |
| HHLL_TREND:DXY             | 'B13'  |


### col(M,N,O,P):
| (index) | Values |
| --- | --- |
| HSI     | 'C1'   |
| HHI     | 'C2'   |
| HTI     | 'C3'   |


### col(R):
| (index) | Values |
| --- | --- |
| hsi     | 'D1'   |
| hssi    | 'D2'   |
| hsmsi   | 'D3'   |









DESC:
```
A: 'time'               // 時間
B: 'hsiClose'           // HSI CLOSE
C: 'indUpList'          // 溢放量的板塊
D: 'indDnList'          // 折放量的板塊
E: 'indABList'          // 主买的板塊
F: 'indASList'          // 主卖的板塊
G: 'isHsiSurge'         // 放量 (6, 7, 8 級的放量)
L: 'stockVolPer'        // 前幾天對比的量百分比
M: 'buyList',           // 主買的指數
N: 'sellList',          // 主賣的指數
O: 'upResisList',       // 向上阻力的指數
P: 'dnResisList',       // 向下阻力的指數
Q: 'isMktCapLargeDiff'  // 大小盘是否有大差異
R: 'mktCapD7SurgeList'  // 大小盘有大差異且放量的SYMBOL

H: 'extUpToDnList'      // 由升轉跌的產品
I: 'extDnToUpList'      // 由跌轉升的產品
J: 'extKeepUpList'      // 持續升的產品
K: 'extKeepDnList'      // 持續跌的產品


```