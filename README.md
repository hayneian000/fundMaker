# fundMaker MVP Overview

**fundMaker** is an app that allows users to create custom index funds by selecting stocks, choosing portfolio weighting and rebalancing strategies, and then back testing their fund's performance over a historical period.

---

## Core Functionality

### Index Fund Builder & Backtesting

Users can:

- Select a list of stock tickers or track an existing index  
- Choose a rebalancing strategy  
- Choose a weighting strategy  
- Select a historical timeframe for testing  
- Run a backtest to view historical performance metrics (e.g., cumulative return, volatility, Sharpe ratio, drawdowns, etc.)

---

### Stock & Index Selection

Users can search and add stocks by:

- Ticker symbol  
- Company name  

> 💡 **Extra Feature**: Include search autocomplete or filters (sector, market cap, country) for a smoother UX.

Users can optionally select a known index (e.g., S&P 500) to start from.

---

### Rebalancing Strategies (Initial Set)

- **Calendar-Based**: Rebalance on a fixed interval (e.g., quarterly, semi-annually)  
- **Threshold-Based**: Rebalance when a holding deviates from its target weight by more than a chosen percentage  

> 💡 **Extra Feature**: Support manual rebalancing (user-triggered) in future versions.

---

### Weighting Strategies (Initial Set)

- **Market Cap Weighted**: Weight proportionally to each stock’s market cap  
- **Equal Weighted**: All stocks receive equal allocation  
- **Fundamental Weighted**: Weighted based on:  
  - Revenue  
  - Earnings  
  - Dividends  

> 💡 **Extra Feature**: Eventually allow users to customize the blend of fundamentals.

---

### Backtesting

Users can:

- Select a custom time range (based on data availability)  
- Run a backtest and view:  
  - Portfolio value over time  
  - Performance vs. benchmark (e.g., S&P 500)  
  - Key stats (return, volatility, drawdown, Sharpe, etc.)  
  - Allocation drift over time  
  - Rebalancing events and effects  

> 💡 **Extra Feature**: Enable export of results as CSV or image.

---

## User Experience & UI

### Sign Up / Sign In

Optional to use the app.

Required only for:
- Posting to leaderboards  
- Saving funds to a user profile  
- Liking or commenting on other users' indexes  

> 💡 **Extra Feature**: Allow anonymous users to try the app with localStorage before committing to an account.

---

### Homepage

Includes:

- Introduction to the app  
- Quick demo or sample index fund builder  
- Top-performing funds from leaderboard  
- Recent or trending user-created indexes  

> 💡 **Extra Feature**: Add an “Explore Funds” section to browse others' creations without needing to sign in.

---

### My Indexes (Dashboard)

- View a list of user-created index funds  
- View/edit/retest saved funds  
- See performance summaries at a glance  

> 💡 **Extra Feature**: Allow cloning and modifying old funds to iterate easily.

---

### Create New Index (Builder Flow)

A step-by-step guided experience:

1. Select Stocks  
2. Choose Weighting Strategy  
3. Choose Rebalancing Strategy  
4. Set Timeframe  
5. Run Backtest  
6. Save & Share (optional)

> 💡 **Extra Feature**: Auto-suggest popular stock groups like “Top 10 Tech Stocks” or “Dividend Aristocrats.”

---

### Leaderboard

Ranked list of user-created index funds by:

- Performance over chosen timeframes (e.g., 1Y, 3Y, max)  
- Likes or popularity  
- Risk-adjusted return (e.g., Sharpe)

Users can:

- Like or comment on indexes  
- View fund details, holdings, rebalancing logic, and backtest data  
- Clone to start building their own variation  

> 💡 **Extra Feature**: Add filters like "Most Liked", "Most Volatile", "Best in Last Month".

---

## Bonus Feature (Subscription Only)

A premium feature available to paying users allows the creation of **live, connected index funds**.

### Brokerage Integration

Users can:

- Connect their fundMaker account to a supported brokerage account
- Automatically sync their custom index fund to their brokerage portfolio

### Automated Portfolio Management

Once connected, the app will:

- Execute trades to match the selected stocks, weights, and rebalancing strategy
- Monitor and rebalance the portfolio according to the user’s chosen strategy (calendar-based or threshold-based)
- Send real-time notifications for actions taken or recommended

> **Note**: Brokerage integration will be a pain.

### Why Subscribe?

This feature provides:

- Hands-free investing based on fully customized index logic
- Guaranteed strategy alignment without manual trading
- Peace of mind with transparency and control over execution

**Subscription Tier Includes:**

- Automated trading & rebalancing  
- Priority support  
- Access to exclusive weighting strategies (e.g., ESG filters, custom metrics, ect)  
- Ability to clone and track top-performing indexes in real time

---

## Future Ideas / Stretch Goals

- Social features: comments, fund discussions  
- Real-time portfolio tracking with live prices  
- Email summaries for watched or owned indexes  
- Comparison tools (side-by-side fund comparisons)  
- Community challenges (e.g., “Best 2023 Tech Fund”)