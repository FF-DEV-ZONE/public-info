# 市场领先行业信号查询接口文档

该接口用于获取指定时间段内的市场领先行业信号数据。

## 1. 接口概览
- **接口地址**: `http://192.168.25.127:8288/index/list`
- **请求方式**: `GET`
- **内容类型**: `application/json`

## 2. 请求参数 (Query Parameters)
| 参数名 | 类型 | 必选 | 示例值 | 说明 |
| :--- | :--- | :--- | :--- | :--- |
| `type` | string | 是 | `market_leading_industry` | 业务数据类型 |
| `key_list` | string | 是 | `signal` | 关键指标列表 |
| `startTime` | string | 是 | `2026-05-07 03:20:00` | 开始时间 (YYYY-MM-DD HH:mm:ss) |
| `endTime` | string | 是 | `2026-05-07 13:40:00` | 结束时间 (YYYY-MM-DD HH:mm:ss) |

## 3. 响应参数说明
### 3.1 核心响应字段
| 字段名 | 类型 | 说明 |
| :--- | :--- | :--- |
| `message` | string | 状态描述信息 |
| `code` | string | 状态码（200 为成功） |
| `results` | array | 结果数据列表 |

### 3.2 Results 数组项结构
| 字段名 | 类型 | 说明 |
| :--- | :--- | :--- |
| `s` | string | 市场代码 (例如: US) |
| `i` | string | 行业代码 (例如: IT) |
| `openTime` | long | 信号开始时间戳 (毫秒) |
| `closeTime` | long | 信号结束时间戳 (毫秒) |
| `uniqueSymbol` | string | 唯一标识符 |

## 4. 响应示例
```json
{
    "message": "操作成功",
    "code": "200",
    "status": "success",
    "results": [
        {
            "s": "US",
            "closeTime": 1778097660000,
            "i": "IT",
            "openTime": 1778097600000,
            "uniqueSymbol": "US"
        }
    ]
}
