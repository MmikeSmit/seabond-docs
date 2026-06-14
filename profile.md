# Profile

Profile is the personal account center in SeaBond. It brings together the user's identity, account value, copy-trading portfolio, unified trading account, open positions, assets, orders, and transaction history in one place.

Use this page to review portfolio performance, manage copy-trading activity, inspect trading records, and update personal profile information.

{% hint style="info" %}
Profile is available only after the user is signed in. If the user is not authenticated, SeaBond will redirect them to the Smart Money page.
{% endhint %}

## Page access

| Destination | URL | Description |
| --- | --- | --- |
| Profile overview | `/profile` | Opens the default Overview section. |
| Copy-trading portfolio | `/profile?tab=copies` | Opens the Copies section directly. |
| Unified trading account | `/profile?tab=perpetuals` | Opens the Perpetuals section directly. |

## Main sections

Profile is organized into three primary sections.

| Section | Purpose |
| --- | --- |
| Overview | A consolidated view of the user's main wallet and copy-trading sub-wallets. |
| Copies | A dedicated view for copy-trading equity, active copy rules, and copy-trading history. |
| Perpetuals | A dedicated view for the user's own unified trading account, positions, assets, orders, and trading history. |

## Overview

The Overview section provides a consolidated account view. It combines the user's main wallet and copy-trading sub-wallets to show overall account value and recent performance.

### Estimated total value

Estimated Total Value represents the user's total account value across the main wallet and copy-trading accounts. The 7-day PnL and chart are based on the aggregated portfolio view.

This section is designed for a high-level portfolio review:

- Total estimated account value
- 7-day PnL
- Portfolio performance chart
- Account-level asset distribution
- Deposit and withdrawal records

### Account view

Account View summarizes account-level balances, PnL, ROI, and risk-related information. It helps users understand how their funds are distributed across direct trading and copy-trading activity.

### Assets

The Assets tab lists the user's spot assets and balances. Users can search assets and optionally hide small balances.

| Control | Description |
| --- | --- |
| Search | Filters assets by keyword. |
| Hide assets below 1 USD | Hides low-value asset rows from the display. |
| Deposit / Withdraw | Opens deposit or withdrawal actions. |

{% hint style="info" %}
Hiding assets below 1 USD is only a display preference. It does not change balances, orders, positions, or trading behavior.
{% endhint %}

### Deposits and withdrawals

The Deposits and Withdrawals tab displays account ledger records related to transfers and balance changes. It is intended for reviewing historical funding activity.

## Copies

The Copies section is dedicated to copy-trading activity. It separates copy-trading accounts from the user's main wallet so that copied positions, copied equity, and copy-trading history can be reviewed independently.

{% hint style="warning" %}
Copy trading may result in losses. Historical trader performance, Smart Money labels, or previous copy-trading results do not guarantee future returns.
{% endhint %}

### Copy-trading equity

Copy Trading Equity shows the current equity across the user's copy-trading sub-wallets. This value is isolated from the user's main wallet.

The section includes:

| Metric | Description |
| --- | --- |
| Copy Trading Equity | Total equity across copy-trading sub-wallets. |
| 7D PNL | Recent copy-trading performance over the selected period. |
| Available Margin | Margin currently available for copy-trading activity. |
| PnL | Net copy-trading PnL. |
| Unrealized PnL | Open unrealized PnL across copied positions. |

### Active copying

The Copying tab lists active copy-trading rules. If active rules exist, the tab displays the number of active items.

Users can:

- Create a new copy trade.
- Review active copy-trading rules.
- Stop all active copy trades.
- Manage individual copy-trading rules from the rule list.

### Copying history

Copying History displays historical copy-trading records, including stopped or closed copy relationships. Use this section to review past copy-trading activity and outcomes.

{% hint style="info" %}
Copy-trading updates are processed asynchronously. After creating, closing, deleting, or adjusting a copy-trading rule, the displayed data may take a short time to fully update.
{% endhint %}

## Perpetuals

The Perpetuals section focuses on the user's own unified trading account. It does not include copy-trading sub-wallets.

Use this section to review direct trading activity, including positions, spot assets, trade history, open orders, funding history, and order history.

### Unified trading summary

The summary panel provides a top-level view of the user's direct trading account.

| Metric | Description |
| --- | --- |
| Total Equity | Estimated equity of the user's main unified trading account. |
| 7D PNL | Recent PnL for the main account. |
| Spot Value | Estimated value of spot assets. |
| MMR | Maintenance margin ratio. |
| Available Margin | Margin available for direct trading. |
| Perps Unrealized PNL | Unrealized PnL from perpetual positions. |
| Spot Unrealized PNL | Unrealized PnL from spot holdings. |

### Positions

The Positions tab displays open perpetual positions. Depending on the position and account state, users may be able to:

- Set or edit TP/SL.
- Close a position.
- Reverse a position.
- Add margin.
- Adjust leverage.

### Assets

The Assets tab displays spot assets held by the main wallet. It supports keyword search and the option to hide small balances.

### Trade history

Trade History shows executed trades. Users can filter records by:

- All
- Long
- Short
- Spot

The Aggregate option can be used to group related fills where supported.

### Open orders

Open Orders displays active orders. Users can filter orders and manage them directly from the table.

Available actions may include:

- Cancel an order.
- Cancel all orders.
- Edit an order.

### Funding history

Funding History displays funding-related records for perpetual positions. It supports filtering by all, long, or short direction.

### Order history

Order History displays historical orders and their statuses. It supports filtering by all, long, short, or spot orders.

## My Profile

The My Profile button opens the Profile tab inside Settings. This area is used to manage personal account information and review account-level fee information.

Users can manage:

| Item | Description |
| --- | --- |
| Avatar | Upload or update the profile avatar. |
| Display name | Update the visible profile name. |
| UID | Copy the user's SeaBond UID. |
| VIP level | View the current VIP level and tier information. |
| Description | Add or update a short profile description. |
| Fees | Review effective maker and taker fees. |

### Avatar requirements

Supported avatar formats:

- JPG
- PNG
- WebP

Maximum file size: 2 MiB.

### Profile description requirements

The profile description must be between 1 and 200 characters. Line breaks are supported. Unsupported control characters cannot be saved.

## Data scope

SeaBond separates portfolio data by account purpose.

| Area | Data scope |
| --- | --- |
| Overview | Main wallet plus copy-trading sub-wallets. |
| Copies | Copy-trading sub-wallets only. |
| Perpetuals | Main wallet unified trading account only. |

This separation helps users distinguish between direct trading performance and copied trading performance.

## Important notes

{% hint style="warning" %}
Trading and copy trading involve financial risk. Users should understand position size, leverage, margin usage, liquidation risk, and personal risk tolerance before trading or copying another wallet.
{% endhint %}

{% hint style="info" %}
Some account data is updated through external systems and asynchronous services. If a recent action is not reflected immediately, refresh the page or wait briefly for the latest account state to synchronize.
{% endhint %}

## FAQ

### Why can't I access Profile?

Profile requires authentication. If the user is not signed in, SeaBond redirects them to the Smart Money page.

### Why is Overview different from Perpetuals?

Overview includes both the main wallet and copy-trading sub-wallets. Perpetuals only shows the main wallet's unified trading account.

### Why did my copy-trading data not update immediately?

Copy-trading changes are processed asynchronously. Creation, closure, deletion, and margin adjustments may take a short time to appear in the interface.

### Does hiding assets below 1 USD affect my balance?

No. It only changes how assets are displayed. It does not affect balances, positions, orders, or trading activity.

### Where can I update my profile information?

Open Profile, select Overview, and click My Profile to access profile settings.

