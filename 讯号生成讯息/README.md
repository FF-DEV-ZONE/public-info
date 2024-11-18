# 讯号讯息

### 讯号对应数据
- TREND
  - HK50.21 @20241108
    - BULLISH: 中空/互多
    - BEARISH: 中多/互空
    - source: FORECAST_MODEL (isHedgedShPosition, isHedgedLnPosition, isTrsLn, isTrsSh)
    - - [Live Data](http://192.168.25.240:3020/symbolmonitor/infolist/FORECAST_MODEL?header=tsFm,tsFmF,isHedgedShPosition,isHedgedLnPosition,isTrsLn,isTrsSh), [DEV Data](http://192.168.25.201:3050/symbolmonitor/infolist/FORECAST_MODEL?header=tsFm,tsFmF,isHedgedShPosition,isHedgedLnPosition,isTrsLn,isTrsSh)
  - ~~HK50.35~~
- TURNING_POINT
  - HK50.35
    - source: FORECAST_MODEL (isResisUp_20241029, isResisDn_20241029)
    - [Live Data](http://192.168.25.240:3020/symbolmonitor/infolist/FORECAST_MODEL?header=tsFm,tsFmF,isResisUp_20241029,isResisDn_20241029), [DEV Data](http://192.168.25.201:3050/symbolmonitor/infolist/FORECAST_MODEL?header=tsFm,tsFmF,isResisUp_20241029,isResisDn_20241029)
- TREND_TO_HOLD
  - HK50.70 @20241108
    - FORECAST_MODEL_MULTI_LOGIC (isKeepTrendLn, isKeepTrendSh => trendToHoldDir)
    - [Live Data](http://192.168.25.240:3020/symbolmonitor/infolist/STRUCTURE_ZYJ_GROUP?header=tsFm,tsFmF,isKeepTrendLn,isKeepTrendSh,trendToHoldDir), [DEV Data](http://192.168.25.201:3050/symbolmonitor/infolist/STRUCTURE_ZYJ_GROUP?header=tsFm,tsFmF,isKeepTrendLn,isKeepTrendSh,trendToHoldDir)
  - ~~HK50.33~~
- ACTIVE_BUY_SELL_DIRECTION
  - HK50.70 @20241108
    - BULLISH: isTurningToLn == true
    - BEARISH: isTurningToSh == true
    - source: FORECAST_MODEL_MULTI_LOGIC (isTurningToLn, isTurningToSh)
    - [Live Data](http://192.168.25.240:3020/symbolmonitor/infolist/STRUCTURE_ZYJ_GROUP?header=tsFm,tsFmF,isTurningToLn,isTurningToSh), [DEV Data](http://192.168.25.201:3050/symbolmonitor/infolist/STRUCTURE_ZYJ_GROUP?header=tsFm,tsFmF,isTurningToLn,isTurningToSh)
    - <a href="http://192.168.25.240:3020/symbolmonitor/infolist/STRUCTURE_ZYJ_GROUP?header=tsFm,tsFmF,isTurningToLn,isTurningToSh" target="_blank">View Data</a>
  - ~~HK50.35~~
- TREND_W (牛熊計算的 TREND)
  - HK50.80 @20241114
    - BULLISH: 中空/互多 (isHedgedShPosition == true)
    - BEARISH: 中多/互空 (isHedgedLnPosition == true)
    - source: FORECAST_MODEL_MULTI_LOGIC (isHedgedShPosition, isHedgedLnPosition)
    - - [Live Data](http://192.168.25.240:3020/symbolmonitor/infolist/FORECAST_MODEL_MULTI_LOGIC?symbol=HSI_WARRANT&header=tsFm,tsFmF,isHedgedShPosition,isHedgedLnPosition), [DEV Data](http://192.168.25.201:3050/symbolmonitor/infolist/FORECAST_MODEL_MULTI_LOGIC?symbol=HSI_WARRANT&header=tsFm,tsFmF,isHedgedShPosition,isHedgedLnPosition)
- TURNING_POINT_W (牛熊計算的 TURNING_POINT)
  - HK50.80 @20241114
    - source: FORECAST_MODEL_MULTI_LOGIC (isResisUp, isResisDn)
    - [Live Data](http://192.168.25.240:3020/symbolmonitor/infolist/FORECAST_MODEL_MULTI_LOGIC?symbol=HSI_WARRANT&header=tsFm,tsFmF,isResisUp,isResisDn), [DEV Data](http://192.168.25.201:3050/symbolmonitor/infolist/FORECAST_MODEL_MULTI_LOGIC?symbol=HSI_WARRANT&header=tsFm,tsFmF,isResisUp,isResisDn)



---
### Tradingview 编码对应表
| 编码 | 描述 | CODE | 晚上 | CODE |
| --- | --- | --- | --- | --- |
|HK50.21| ETF, 期貨折溢價排列計算 | FORECAST_MODEL |  |  |
|HK50.37| 打出不同行業的多空的方向 | INDUSTRY_SECTOR_PATTERN |  |  |
|HK50.38| 以行業比重計算多空的方向 | INDUSTRY_SECTOR_PATTERN_SUMMARY |  |  |
|HK50.40| 港股通接近恒生指数 | HSI_GGT_HSI_LIKE_EI | 港股盤後 | US_PRE_MARKET |
|HK50.41| HSI证券AH股 | HSI_SECURITY_EI | 美股 (CD, IT, 綜合) | US_MARKET_COMPOSITE |
|HK50.42| HSI非银港元 | HSI_NON_BANK_EI | MCHI, FXI, YANG, YINN vs HXC | US_MARKET_ZGG_ETF |
|HK50.43| HSI银行AH股 | HSI_BANK_EI | | |
|HK50.44| 能源业AH股 | HSI_ENERGY_EI | | |
|HK50.45| 生物科技H股 | HSI_BIOTECH_EI | | |
|HK50.46| 可选消费AH股 | HSI_CD_AH_EI | | |
|HK50.47| HSI_futures_HKEX交易时间内_zyj | FUTURE_HKEX_DAY_TIME | | |
|HK50.48| 港股通科技股接近科技指数 | HSI_GGTIT_HTI_LIKE_EI | | |
|HK50.49| 港股通国企高息接近国企指数 | HSI_GGT_HIGH_DIV_HHI_LIKE_EI | | |
|HK50.70| 恒生內部多個折溢價計算 | STRUCTURE_ZYJ_GROUP | | |
|HK50.80| 牛熊折溢價計算 | FORECAST_MODEL_MULTI_LOGIC <br /> WARRANT_VS_INDEX_SEQ_COMPARE | | |

