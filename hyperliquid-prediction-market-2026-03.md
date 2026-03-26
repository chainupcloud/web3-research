# Hyperliquid 预测市场调研报告（2026年3月）

---

## 一、核心提案：HIP-4 Outcome Trading

2026年2月2日，Hyperliquid 发布 HIP-4 提案，正式宣布进军预测市场。HIP-4 引入"Outcome（结果合约）"原语，核心特性：

- **全额抵押**：无杠杆、无爆仓，持仓全额资金覆盖
- **固定区间结算**：合约在固定价格区间内结算（如 YES=1 USDH / NO=0 USDH）
- **有时效性**：带到期日的合约，区别于永续合约
- **非线性收益**：类期权的收益曲线

适用场景：二元预测市场（Yes/No）、有限风险的类期权工具、各类事件结果交易。

---

## 二、当前进展（2026年3月）

| 里程碑 | 状态 |
|--------|------|
| HIP-4 提案发布 | ✅ 2026年2月2日 |
| Testnet 上线 | ✅ 2026年3月（已可测试） |
| 官方 Canonical 市场 | 🔄 开发中，上线日期未定 |
| Permissionless 部署 | 📋 待用户反馈后推进 |
| Mainnet 正式上线 | 🗓️ 2026年内（无具体时间） |

**首批市场**将由官方部署，基于客观数据源结算，以 **USDH**（Hyperliquid 原生稳定币）计价。

---

## 三、技术架构与生态协同

HIP-4 与已有基础设施深度整合：

- **Portfolio Margin**（组合保证金）：Outcome 合约与永续合约共享同一保证金体系，提升资金效率
- **HyperEVM**：2026年3月1日已主网上线，为 Outcome 合约提供可编程性支持，开发者可在此基础上构建应用
- **HyperCore**：底层撮合引擎，提供高性能链上撮合能力

---

## 四、与 Polymarket 对比

| 维度 | Hyperliquid HIP-4 | Polymarket |
|------|------|------|
| 合约类型 | 二元 + 连续区间（通用原语） | 主要为二元 Yes/No |
| 结算代币 | USDH | USDC |
| KYC | 无 | 无（US版有限制） |
| 杠杆/爆仓 | 无，全额抵押 | 无 |
| 与衍生品整合 | ✅ 共享保证金 | ❌ 独立平台 |
| 无许可部署 | 规划中 | ✅ 已支持 |
| 美国用户 | ❌ 不可用 | ✅ 新上线US版（有限） |
| 当前状态 | Testnet | Mainnet |

---

## 五、市场影响

- HYPE 代币在 HIP-4 发布后上涨约 **10-20%**
- 预测市场将为 Hyperliquid 带来 **每月额外 $28-40 亿** 交易量
- Hyperliquid 2026年1月总交易量已达 **$2250亿**
- HyperEVM 主网上线后，日交易量峰值达 **340万笔**

---

## 六、核心风险与挑战

1. **地理限制**：不支持美国、加拿大等主要市场，限制用户规模
2. **主网时间未定**：仅承诺"2026年内"，市场催化剂存在不确定性
3. **预言机依赖**：结算依赖客观数据源，争议处理机制仍需验证
4. **竞争压力**：Polymarket 已推出美国版，先发优势明显

---

## 七、Testnet 实测指南（2026年3月）

### 前提条件
- EVM 兼容钱包（MetaMask、Rabby 等），且**主网钱包需有存款历史**，否则 Faucet 无法使用
- 非美国/加拿大用户

### 操作步骤

**1. 进入 Testnet**
- 直接访问 `app.hyperliquid-testnet.xyz`（独立测试网域名），连接钱包

**2. 领取测试资金**
- 点击 `Faucet`，获得 1,000 模拟 USDC（每账户仅限一次）

**3. 将 USDC 换成 USDH**
- Outcome 合约**只接受 USDH** 计价
- 进入 Spot 现货板块，找到 `USDH/USDC` 交易对，买入 USDH

**4. 查找 Outcome 合约**
- 进入交易页面，点击**币对选择下拉菜单**，切换到 `Predict` 分类
- 即可看到所有可交易的预测市场合约
- 直接访问示例市场：`app.hyperliquid-testnet.xyz/trade/who-will-win-the-hl-100-meter-dash-hypurr`

### 首批市场品种
- BTC 价格二元期权（如"BTC 3月31日前突破 $120,000？"）
- HYPE 价格相关合约
- 均为每日到期 Yes/No 合约，USDH 计价

### 注意事项
- 参与 Testnet 可能计入**第三季空投资格**
- 底部面板持仓区可能有 `Prediction` 标签用于查看仓位

---

## 八、总结

Hyperliquid HIP-4 是目前 DeFi 领域最具潜力的预测市场基础设施之一。其核心优势在于**与高流动性衍生品生态的深度整合**——Outcome 合约、永续合约、组合保证金三者协同，将创造独特的交易体验。目前处于 Testnet 阶段，主网上线后有望显著扩大 Hyperliquid 的产品边界和用户规模。

---

## 参考来源

- [CoinDesk: HIP-4 proposal](https://www.coindesk.com/markets/2026/02/02/hyperliquid-s-hype-higher-by-10-on-plans-to-add-prediction-markets-and-options)
- [The Block: Hyperliquid tests Outcomes](https://www.theblock.co/post/388023/hyperliquid-outcome-prediction-markets-limited-risk-options-trading)
- [CoinLedger: How to Trade HIP-4 (Testnet)](https://coinledgerinsight.com/en/2026/03/12/hyperliquid-hip4-outcome-trading-prediction-market-guide/)
- [QuickNode: What is HIP-4? Outcome Contracts Explained](https://blog.quicknode.com/hip4-hyperliquid-outcome-contracts/)
- [Hyperliquid官方X公告: HIP-4](https://x.com/HyperliquidX/status/2018327360723202167)
- [TechFlow: HIP-4 深度分析](https://www.techflowpost.com/en-US/article/30220)
- [KuCoin: $225B Volume + HIP-4](https://www.kucoin.com/news/flash/hyperliquid-processes-225-billion-in-volume-as-hip-4-aims-to-boost-prediction-markets)
