# 2.2 Stock Market Structure

<span class="badge badge-data">Market Data</span> <span class="badge badge-quant">Quantitative Focus</span>

Comprehensive overview of Vietnam's three-tier stock market structure, major indices, sector composition, and key market characteristics for quantitative analysis.

## Exchanges Overview

Vietnam operates a three-tier stock exchange system, each serving different market segments:

| Exchange | Established | Listed Cos | Market Cap | Avg Daily Volume | Main Characteristics |
|----------|-------------|-----------|------------|-----------------|---------------------|
| **HOSE** | 2000 | 400+ | $180B | $600M | Blue chips, high liquidity |
| **HNX** | 2005 | 350+ | $45B | $120M | Mid-caps, government bonds |
| **UPCoM** | 2009 | 800+ | $25B | $80M | SMEs, unlisted public companies |

### Ho Chi Minh Stock Exchange (HOSE)

**Overview**:
- **Focus**: Large-cap, blue-chip companies
- **Listing Requirements**: High (min capital VND 80B / ~$3.3M)
- **Trading**: Continuous auction with price bands
- **Settlement**: T+2
- **Key Sectors**: Banking (35%), Real Estate (18%), Manufacturing (15%)

**Top 10 HOSE Stocks by Market Cap** (Feb 2025):

| Ticker | Company | Sector | Market Cap | Avg Daily Vol | FOL Status |
|--------|---------|--------|-----------|--------------|------------|
| VCB | Vietcombank | Banking | $18B | $50M | 85% (near limit) |
| BID | BIDV | Banking | $12B | $35M | 78% |
| VHM | Vinhomes | Real Estate | $11B | $30M | At limit (100%) |
| VIC | Vingroup | Conglomerate | $10B | $45M | 92% |
| GAS | PetroVietnam Gas | Energy | $8B | $25M | 45% |
| VNM | Vinamilk | Consumer | $7B | $20M | At limit (100%) |
| HPG | Hoa Phat Steel | Materials | $7B | $28M | 73% |
| CTG | VietinBank | Banking | $6.5B | $22M | 81% |
| MSN | Masan Group | Consumer | $6B | $18M | 95% |
| VPB | VPBank | Banking | $5.5B | $20M | 88% |

**Liquidity Concentration**:
- Top 30 stocks: 70% of daily volume
- Top 100 stocks: 90% of daily volume
- Long tail: 300+ stocks with <$1M daily volume

### Hanoi Stock Exchange (HNX)

**Overview**:
- **Focus**: Mid-cap companies, government bonds
- **Listing Requirements**: Lower than HOSE (min capital VND 30B / ~$1.25M)
- **Trading**: Similar to HOSE, but lower liquidity
- **Settlement**: T+2
- **Key Sectors**: Construction, Materials, Services

**Characteristics**:
- Less institutional participation
- Higher retail investor concentration
- More volatile than HOSE
- Opportunities for alpha in less-researched names

**Notable HNX Stocks**:
- **SHS**: Securities (brokerage house)
- **PVS**: Petroleum services
- **VCS**: Construction
- **CEO**: Real estate, tourism

### Unlisted Public Company Market (UPCoM)

**Overview**:
- **Focus**: SMEs, companies preparing for HOSE/HNX listing
- **Listing**: Minimal requirements
- **Trading**: OTC platform (not full exchange)
- **Liquidity**: Very limited

**Characteristics**:
- High bid-ask spreads (50-200bps)
- Irregular trading (some stocks don't trade daily)
- Information asymmetry (limited research coverage)
- Alpha opportunities for skilled traders

**Use Cases**:
- Pre-IPO plays (companies upgrading to HOSE/HNX)
- Special situations (restructurings, M&A)
- Arbitrage (cross-listing to main exchanges)

## Major Indices

### VN-Index (Ho Chi Minh Stock Index)

**Overview**:
- **Base**: 100 (July 28, 2000)
- **Current Level**: ~1,250 (Feb 2025)
- **Constituents**: All HOSE-listed stocks
- **Weighting**: Free-float adjusted market cap
- **Rebalancing**: Quarterly

**Historical Performance**:

| Period | Return (Annualized) | Volatility | Sharpe Ratio | Max Drawdown |
|--------|-------------------|------------|--------------|--------------|
| 2000-2024 | +12.5% | 24% | 0.52 | -65% (2008) |
| 2010-2024 | +9.8% | 18% | 0.54 | -38% (2020) |
| 2015-2024 | +11.2% | 20% | 0.56 | -30% (2022) |
| 2020-2024 | +15.3% | 22% | 0.70 | -22% (2022) |

**Key Observations**:
- Long-term growth driven by GDP
- High volatility (typical for frontier/emerging markets)
- Positive Sharpe ratio despite volatility
- Deep drawdowns during crises (2008, 2020, 2022)

### VN30 (VN30 Index)

**Overview**:
- **Launch**: 2012
- **Constituents**: 30 largest, most liquid HOSE stocks
- **Weighting**: Free-float adjusted market cap
- **Rebalancing**: Quarterly (March, June, Sept, Dec)
- **Derivatives**: VN30 futures available

**Characteristics**:
- Highly liquid (70%+ of HOSE volume)
- Institutional benchmark
- Lower volatility than VN-Index
- Good for large-cap momentum strategies

**VN30 Composition by Sector** (Feb 2025):

| Sector | Weight | # Stocks | Key Holdings |
|--------|--------|----------|--------------|
| Banking | 38% | 7 | VCB, BID, CTG, VPB, TCB |
| Real Estate | 22% | 5 | VHM, VIC, NVL, PDR |
| Manufacturing | 12% | 4 | HPG, GVR, HSG |
| Consumer | 10% | 3 | VNM, MSN, SAB |
| Energy | 8% | 2 | GAS, PLX |
| Utilities | 5% | 2 | POW, GEG |
| Telecom | 3% | 1 | FPT |
| Other | 2% | 6 | Various |

**Index Rebalancing Effects**:
- Additions: +3-5% on announcement, +2-3% at inclusion
- Deletions: -5-8% on announcement, -3-5% at exclusion
- Front-running opportunity (announce 2 weeks before effective date)

### HNX-Index

**Overview**:
- **Base**: 100 (Jan 2, 2009)
- **Current Level**: ~250 (Feb 2025)
- **Constituents**: All HNX-listed stocks
- **Weighting**: Market cap

**Performance**:
- Historically lagged VN-Index
- Higher volatility, lower liquidity
- Less institutional coverage
- Opportunities for stock-pickers

### HNX30

**Overview**:
- Top 30 HNX stocks
- Similar to VN30 but for mid-caps
- Lower correlation with VN30 (0.65)
- Diversification benefits

## Market Capitalization & Sector Breakdown

### Total Market Overview (All Exchanges)

| Metric | Value | % of GDP |
|--------|-------|----------|
| **Total Market Cap** | $250B | 70% |
| **HOSE** | $180B | 50% |
| **HNX** | $45B | 13% |
| **UPCoM** | $25B | 7% |

**Sector Distribution** (HOSE + HNX):

| Sector | Market Cap | % of Total | # Companies | Top Players |
|--------|-----------|-----------|-------------|-------------|
| **Banking & Finance** | $87B | 35% | 45 | VCB, BID, CTG, VPB |
| **Real Estate** | $45B | 18% | 85 | VHM, VIC, NVL, DXG |
| **Manufacturing** | $38B | 15% | 120 | HPG, GVR, HSG, DCM |
| **Consumer Goods** | $25B | 10% | 60 | VNM, MSN, SAB, KDC |
| **Energy** | $20B | 8% | 25 | GAS, PLX, PVD |
| **Technology** | $13B | 5% | 40 | FPT, VGI, CMG |
| **Utilities** | $12B | 5% | 15 | POW, GEG, NT2 |
| **Healthcare** | $5B | 2% | 30 | DHG, DMC, IMP |
| **Other** | $5B | 2% | 180 | Various |

### Sector Characteristics for Quant Analysis

| Sector | Avg Market Cap | Liquidity | Volatility | Momentum | Value Factor |
|--------|---------------|-----------|------------|----------|--------------|
| Banking | $4B | High | Moderate (18%) | Works | P/B effective |
| Real Estate | $1.5B | High | High (28%) | Strong | Cyclical |
| Manufacturing | $800M | Moderate | Moderate (22%) | Moderate | P/E works |
| Consumer | $1.2B | Moderate | Low (15%) | Low | Quality factor |
| Energy | $2B | Moderate | High (25%) | Commodity-linked | P/E less useful |
| Technology | $600M | Low | High (30%) | Strong | Growth over value |

## Trading Characteristics

### Trading Hours

| Session | Time (ICT) | Notes |
|---------|-----------|-------|
| **Opening Auction** | 09:00-09:15 | Order matching for opening price |
| **Continuous Trading (AM)** | 09:15-11:30 | Main trading session |
| **Lunch Break** | 11:30-13:00 | No trading |
| **Continuous Trading (PM)** | 13:00-14:30 | Afternoon session |
| **Closing Auction** | 14:30-14:45 | Order matching for closing price |

**Put-Through Session** (Large Block Trades): 14:45-15:00

### Order Types

1. **Limit Order (LO)**: Specific price, FIFO matching
2. **Market Order (MP/MAK)**: Best available price (limited to ±7% reference)
3. **ATO/ATC**: At The Open / At The Close (auction sessions)
4. **Put-Through**: Pre-negotiated blocks (min 5% ADV or 10B VND)

### Price Bands & Circuit Breakers

**Daily Price Limits**:
- **±7%** from reference price (previous day's close)
- **±10%** for stocks in "under supervision" category
- No trading halts (unlike US) - just price limits

**Implications for Quant Trading**:
- Momentum can be capped by limits
- Gap-up/down stocks often hit limit for days
- Limit orders at ±6.5% can capture extremes

### Market Microstructure

**Tick Size**:
- VND 10 (0.01 VND) for stocks <VND 10,000
- VND 50 for stocks VND 10,000-50,000
- VND 100 for stocks >VND 50,000

**Lot Size**:
- **Standard**: 100 shares
- **Odd Lot**: <100 shares (traded at end of day)

**Settlement**:
- **T+2** for most stocks (trade date + 2 business days)
- **T+3** for some (check exchange rules)
- **Cash Upfront**: Some brokers require 100% cash before trading

## Historical Index Performance

### VN-Index Long-term Chart (2000-2024)

**Major Bull Markets**:
1. **2000-2007**: +1,070% (100 → 1,170) - Vietnam joins WTO
2. **2009-2011**: +105% (235 → 483) - Post-GFC recovery
3. **2012-2018**: +135% (351 → 825) - Steady growth, reforms
4. **2020-2021**: +48% (960 → 1,420) - COVID recovery, liquidity surge

**Major Bear Markets**:
1. **2007-2009**: -70% (1,170 → 235) - Global Financial Crisis
2. **2018-2020**: -16% (989 → 832) - Trade war, COVID
3. **2022**: -33% (1,500 → 1,006) - Fed tightening, global slowdown

### VN-Index vs Regional Peers (Cumulative Returns 2015-2024)

| Index | Total Return | Annualized | Volatility | Sharpe | Correlation w/ VN |
|-------|-------------|------------|------------|--------|------------------|
| **VN-Index** | +182% | +11.2% | 20% | 0.56 | 1.00 |
| **SET (Thailand)** | +45% | +4.3% | 18% | 0.24 | 0.62 |
| **PCOMP (Philippines)** | +58% | +5.3% | 16% | 0.33 | 0.55 |
| **JCI (Indonesia)** | +72% | +6.3% | 19% | 0.33 | 0.60 |
| **MSCI EM** | +65% | +5.8% | 17% | 0.34 | 0.48 |
| **S&P 500** | +225% | +13.1% | 15% | 0.87 | 0.35 |

**Key Takeaways**:
- Vietnam outperformed regional peers and EM index
- Higher volatility than developed markets
- Lower correlation with US (diversification benefit)
- Moderate correlation with ASEAN (regional linkage)

## Market Depth & Liquidity Analysis

### Liquidity Tiers

**Tier 1: Highly Liquid** (VN30 core)
- Daily Volume: $20M+
- Bid-Ask Spread: 5-15 bps
- Market Impact: <10 bps for $1M trade
- Examples: VCB, VIC, VHM, HPG

**Tier 2: Liquid** (VN30 periphery, large HOSE)
- Daily Volume: $5M-20M
- Bid-Ask Spread: 15-30 bps
- Market Impact: 10-25 bps for $500K trade
- Examples: CTG, MSN, PLX

**Tier 3: Moderate** (Mid-cap HOSE, top HNX)
- Daily Volume: $1M-5M
- Bid-Ask Spread: 30-60 bps
- Market Impact: 25-50 bps for $200K trade
- Examples: Various mid-caps

**Tier 4: Illiquid** (Small HOSE, most HNX/UPCoM)
- Daily Volume: <$1M
- Bid-Ask Spread: 60-200 bps
- Market Impact: >50 bps even for small trades
- Examples: Long tail of small-caps

### Order Book Depth

**Typical Order Book** (VCB, large-cap):
```
Bid                              Ask
Price   | Volume (sh) | Count   |  Price  | Volume (sh) | Count
--------+-------------+---------+---------+-------------+-------
106,500 | 45,000      | 23      | 106,600 | 38,000      | 19
106,400 | 62,000      | 31      | 106,700 | 52,000      | 28
106,300 | 78,000      | 42      | 106,800 | 69,000      | 35
106,200 | 95,000      | 58      | 106,900 | 81,000      | 41
106,100 | 125,000     | 73      | 107,000 | 105,000     | 54
```

**Observations**:
- Reasonable depth in VN30 stocks
- Fragmented (many small orders)
- Thin beyond 5 price levels
- Market orders can move price

## Quantitative Characteristics

### Factor Performance (2015-2024)

| Factor | Annualized Return | Sharpe | Best Months | Worst Months |
|--------|------------------|--------|-------------|--------------|
| **Momentum (12M)** | +8.2% | 1.15 | 58% | 42% |
| **Value (P/B)** | +5.1% | 0.72 | 55% | 45% |
| **Quality (ROE)** | +6.3% | 0.88 | 61% | 39% |
| **Size (Small-cap)** | +3.8% | 0.54 | 52% | 48% |
| **Low Volatility** | +4.5% | 0.91 | 59% | 41% |

**Multi-factor Strategy** (Momentum + Quality):
- **Return**: +12.5% annualized
- **Sharpe**: 1.32
- **Max DD**: -22%
- **Win Rate**: 64%

### Seasonality Patterns

**Monthly Returns (Average 2015-2024)**:

| Month | Avg Return | Win % | Best for |
|-------|-----------|-------|----------|
| **January** | +4.2% | 70% | Momentum, Tet rally |
| February | +2.1% | 60% | Post-Tet continuation |
| March | +0.5% | 55% | Neutral |
| April | +1.8% | 58% | AGM season |
| May | -0.3% | 48% | Weak |
| June | +0.8% | 52% | Index rebalancing |
| July | +1.2% | 56% | Mid-year reporting |
| August | -0.5% | 47% | Weak |
| September | +0.9% | 54% | Index rebalancing |
| October | -1.1% | 45% | Historically weak |
| November | +2.5% | 62% | Year-end window dressing |
| **December** | +3.8% | 68% | Strong year-end |

**Trading Strategy**:
- Long: January, December, November (Tet + year-end effects)
- Neutral/Short: May, August, October
- Tilt portfolio seasonally

---

**Next**: [Core Regulations](../regulatory/core-regulations.md) - FOL, trading rules, compliance

**Related**:
- [Historical Performance](../quant/historical-performance.md) - Detailed backtests
- [Liquidity Metrics](../microstructure/liquidity-metrics.md) - Execution analysis
- [Data Sources](../infrastructure/data-sources.md) - Where to get index data
