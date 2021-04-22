---
order: 5
title: 常见问题
---
# 常见问题

### 1、怎么判断一个字段是维度还是指标

每一个图表的数据都由 **维度** 和 **指标** 组成。
- **维度** 是指数据的属性。
- **指标** 是量化衡量标准。

|  日期      | 页面名称 |  访问量  | 访客数 |
|  -------  | ------- |  -----  | ----  |
| 20200101  | 首页     |  100    | 50    |
| 20200101  | 登录页   |  50    | 25    |
| 20200102  | 首页     |  120    | 60    |
| 20200102  | 登录页   |  60    | 30    |
| 20200103  | 首页     |  140    | 70    |
| 20200103  | 登录页   |  70    | 35    |
| 20200104  | 首页     |  160    | 80    |
| 20200104  | 登录页   |  80    | 40    |

像上面这一份数据中，`日期` 和 `页面名称` 是 **维度**，`访问量` 和 `访客数` 是 **指标**。

*简单来看，枚举值、时间类一般是**维度**，数字一般是**指标**。*

### 2、图表有数据不展示

<img src="https://img.alicdn.com/imgextra/i2/O1CN011ro0R824CdjdEdkUC_!!6000000007355-2-tps-1610-754.png" alt="图表有数据不展示" width="600"/>

可能是维度字段的数据有空值，如 `null`、`undefined` 等，请手动筛一下数据。