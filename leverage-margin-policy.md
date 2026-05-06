---
layout: default
title: Leverage and Margin Policy
effective_date: 1 March 2018
last_updated: 6 May 2026
---

This Leverage and Margin Policy (the "Policy") is issued by **Kohle Capital Markets Limited** (the "Company", "we", "us", or "our") and sets out the framework governing leverage, margin requirements, margin calls, and position close-out procedures applicable to leveraged trading through digital services operated under the **KCM Trade** brand (the "Services").

This Policy forms part of the Company's client documentation framework and should be read together with the [Risk Disclosure Statement]({{ '/risk-disclosure.html' | relative_url }}), [Order Execution Policy]({{ '/order-execution-policy.html' | relative_url }}), [Client Fund Protection]({{ '/client-fund-protection.html' | relative_url }}), and [Terms of Service]({{ '/terms-of-service.html' | relative_url }}).

> **Important Risk Warning:** Leveraged trading involves a high degree of risk. Your losses may exceed your initial deposit. You should not trade with funds you cannot afford to lose. Please read the [Risk Disclosure Statement]({{ '/risk-disclosure.html' | relative_url }}) carefully before trading.

---

## 1. What is Leverage?

Leverage enables users to open and maintain positions in financial markets with a deposit (margin) that is a fraction of the total notional value of the position.

For example, leverage of 1:100 means that a margin deposit of USD 1,000 controls a position with a notional value of USD 100,000.

While leverage can amplify returns on profitable trades, it equally amplifies losses on unprofitable trades. Losses may exceed the amount deposited as margin.

---

## 2. Leverage Ratios

Maximum leverage ratios vary by asset class and are set by the Company at its discretion, subject to the licensing conditions of the **Financial Services Commission of Mauritius (FSC Mauritius)** and applicable regulatory requirements.

Indicative maximum leverage ratios by product category are set out in the Company's **Product Specification**, available at:

[Product Specification (PDF)](https://mt5.kohlecapital.com/uploads/public/company-documents/2023/08/28/2ecbc2a508df38127f6d132de7b90400.pdf){:target="_blank" rel="noopener noreferrer"} (v4)

| Asset Class | Indicative Maximum Leverage | Notes |
|---|---|---|
| **Major Foreign Exchange Pairs** | Up to 1:500 | Subject to instrument-specific limits |
| **Minor / Exotic Foreign Exchange Pairs** | Up to 1:200 | Higher spread and overnight cost |
| **Major Stock Indices (CFDs)** | Up to 1:200 | Subject to instrument-specific limits |
| **Individual Equity CFDs** | Up to 1:20 | Higher margin requirement applies |
| **Commodities (CFDs)** | Up to 1:100 | Varies by commodity |
| **Cryptocurrencies (CFDs)** | Up to 1:5 | Subject to high volatility adjustments |
| **Bonds (CFDs)** | Up to 1:100 | Subject to instrument-specific limits |

> **Note:** The above figures are indicative maximum leverage levels under normal market conditions. Actual leverage available on any given instrument at any given time may be lower, including as a result of market volatility adjustments, account type restrictions, or the Company's risk management decisions. Current leverage ratios are always displayed in the trading platform prior to order placement.

The Company reserves the right to adjust leverage ratios at any time, including without prior notice, in response to:

- Extreme market volatility or abnormal market conditions
- Regulatory direction or FSC guidance
- The Company's internal risk management requirements
- Approaching economic data releases, central bank announcements, or other scheduled market events

---

## 3. Margin Requirements

### 3.1 Initial Margin

To open a leveraged position, users must have sufficient **free margin** in their account. The initial margin requirement is the minimum collateral required to open a new position, calculated as:

$$\text{Initial Margin} = \frac{\text{Notional Position Value}}{\text{Leverage Ratio}}$$

For example, a position of 1 lot on EUR/USD with a notional value of USD 100,000 at leverage 1:100 requires an initial margin of USD 1,000.

### 3.2 Maintenance Margin

Once a position is open, the user must maintain a minimum level of equity in their account relative to the margin used. This is referred to as the **maintenance margin** or **margin maintenance level**.

The maintenance margin level is the minimum percentage of used margin that must be maintained in the account as equity to prevent automatic position close-out.

### 3.3 Equity, Margin Level, and Free Margin

| Term | Definition |
|---|---|
| **Balance** | Total funds in the account, not accounting for open unrealised P&L |
| **Equity** | Balance ± unrealised profit/loss on all open positions |
| **Used Margin** | Total margin allocated to all currently open positions |
| **Free Margin** | Equity minus Used Margin; the amount available to open new positions |
| **Margin Level (%)** | (Equity ÷ Used Margin) × 100 |

A margin level of 100% means that equity exactly equals used margin. A margin level above 100% means that free margin is available.

---

## 4. Margin Call

A **margin call** is a notification issued to a user when their margin level falls to or below the **Margin Call Level** specified by the Company.

Upon a margin call:

- The user will be notified through the trading platform, by email, or through other available notification channels
- The user is required to take remedial action by either depositing additional funds or closing some or all open positions to restore the margin level above the required threshold
- The Company does not guarantee that a margin call notification will be received or acted upon in time to prevent automatic position close-out

> **Users must not rely on the receipt of a margin call before taking independent action to manage open positions.** It remains the user's responsibility at all times to monitor account equity and margin levels.

---

## 5. Stop-Out (Automatic Close-Out)

If a user's margin level falls to or below the **Stop-Out Level** specified by the Company, the trading platform will automatically begin closing the user's open positions — starting with the largest loss-making position — until the margin level is restored above the Stop-Out Level.

### 5.1 Stop-Out Execution

- Close-out is executed automatically by the trading platform without prior notice or further margin call
- Positions are closed at the best available market price at the time of close-out
- During periods of extreme volatility or market gapping, the close-out price may be materially worse than the margin trigger price
- The Company is not liable for any losses incurred as a result of automatic close-out

### 5.2 Current Margin Call and Stop-Out Levels

Current Margin Call and Stop-Out Level thresholds are displayed in the user's trading platform and are also available upon request to the Company's customer support team. These levels are subject to change, and users should always refer to the current figures in the platform.

---

## 6. Negative Balance Protection

Under normal market conditions, the Company implements **negative balance protection** measures to limit a user's maximum loss on a closed account to the funds deposited.

Negative balance protection means that following the automatic close-out of all positions, any resulting negative account balance arising from normal market conditions will be reset to zero by the Company, at the Company's expense.

> **Limitations:** Negative balance protection may not apply in the following circumstances:
> - Extreme market volatility, market gapping, or discontinuous price movements (including over weekends or after market close)
> - Force majeure events
> - Abuse of the Services, including market manipulation or exploitation of pricing errors
> - Positions that have not been fully closed out at the time the negative balance arises

Users should not rely on negative balance protection as a risk management strategy. All trading involves the risk of loss and users should only allocate funds they are prepared to lose entirely.

---

## 7. Margin Adjustments and Special Conditions

### 7.1 Increased Margin Requirements

The Company may, at its sole discretion and with or without prior notice, increase margin requirements or reduce available leverage in the following circumstances:

- Major scheduled economic announcements (central bank decisions, employment reports, inflation data)
- Geopolitical events likely to cause significant market volatility
- Instrument-specific corporate events (earnings announcements, dividends, stock splits)
- Concentrated or unusually large positions
- Regulatory direction or FSC guidance

### 7.2 Weekend and Holiday Margin

Leveraged positions held open over weekends, public holidays, or other non-trading periods are subject to market gapping risk. The Company may apply increased margin requirements ahead of such periods.

Users are advised to review open positions and margin levels before market close on Fridays and ahead of public holidays.

### 7.3 Hedged Positions

Where a user holds simultaneously open buy and sell positions in the same instrument (a hedged position), reduced margin requirements may apply in accordance with the hedging margin policy set out in the Product Specification. Hedged positions are not risk-free and may be subject to spread costs and financing charges on both legs.

---

## 8. Account Funding and Margin Deposits

### 8.1 Depositing Margin

Users must ensure their account is funded with sufficient margin before placing orders. Deposits are subject to the processing times and methods described on the Company's platform.

### 8.2 Funding During a Margin Call

If a user wishes to respond to a margin call by depositing additional funds, the user must ensure that the deposited funds are credited to the account before the Stop-Out Level is triggered. Processing times for deposits may not be sufficient to prevent automatic close-out. The Company is not responsible for losses incurred where a deposit is initiated but not yet credited at the time of a close-out.

---

## 9. Product Specification Reference

Current instrument-specific leverage ratios, margin requirements, contract sizes, trading hours, swap rates, and spread information are set out in the Company's **Product Specification**:

[Product Specification (PDF)](https://mt5.kohlecapital.com/uploads/public/company-documents/2023/08/28/2ecbc2a508df38127f6d132de7b90400.pdf){:target="_blank" rel="noopener noreferrer"} (v4)

Users are advised to review the Product Specification before trading. In the event of any inconsistency between this Policy and the Product Specification in respect of a specific instrument, the Product Specification shall prevail.

---

## 10. Amendments

The Company may amend this Policy from time to time to reflect changes in:

- Leverage limits or margin requirements
- Applicable laws or FSC regulatory guidance
- Products, instruments, or operational practices

Material changes will be communicated to users through the Services or by email, in accordance with the notification procedures described in the Terms of Service.

---

## 11. Contact Information

For enquiries relating to margin requirements or account funding, please contact:

**Kohle Capital Markets Limited**  
Email: CS@kcmtrade.com  
Phone: +230 5297 0961  
Website: https://www.kcmtrade.com
