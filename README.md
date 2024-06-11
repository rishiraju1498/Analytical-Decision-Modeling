# Kowri Fintech Application Performance Report

## Overview

This document provides a comprehensive analysis of the Kowri Fintech Application, developed by Sevn, a technology company based in Ghana, West Africa. The report includes information on the company's background, Kowri's features, licensing requirements, app performance metrics, transaction types, fee structure, and a mathematical model for maximizing revenue.

## Company Background

- **Sevn**: A technology company headquartered in Ghana, West Africa.
- **Mission**: Enabling Africa’s growing middle class to live a seamless financial lifestyle through accessible, intuitive, and liberating payment solutions.
- **History**: Formerly known as Dreamoval Limited, founded in 2008 by seven Ashesi University Ghana alumni.
- **Growth**: In the last 15 years, Sevn has become a leader in the African Fintech ecosystem, partnering with entities ranging from small stores to major merchants and government agencies.

## Kowri Application

- **Launch**: February 2023
- **Platforms**: Android and iOS
- **Website**: [www.kowri.app](http://www.kowri.app)

### Features

1. Send money to recipient bank accounts and mobile money wallets.
2. Make insurance payments.
3. Pay in-store and online.

### Payment Sources

- **Debit/Credit card**
- **Mobile money wallet**

### Licensing Requirements

To operate the Kowri app, Sevn Limited needed to be licensed as a Payment Service Provider by the Central Bank of Ghana. The license fees are as follows:

- **Annual License Fee**: $3400.00
- **Capital Deposit**: $167000.00

## Performance Metrics

### Monthly Transaction Data

| Month      | Volume of Transactions | Value of Processed Transactions | Number of Active Users |
|------------|-------------------------|---------------------------------|------------------------|
| March      | 545                     | $12,833                         | 245                    |
| April      | 687                     | $23,750                         | 289                    |
| May        | 1124                    | $100,000                        | 986                    |
| June       | 1839                    | $200,000                        | 1206                   |
| July       | 3424                    | $225,000                        | 1405                   |
| August     | 6500                    | $200,000                        | 1825                   |
| September  | 6834                    | $191,667                        | 1302                   |
| October    | 9452                    | $250,000                        | 1886                   |

### Transaction Types

Since its inception, Kowri customers have dominantly used their apps to send money to mobile money wallets. The table below shows the types of mobile money transactions performed by Kowri customers:

| Transaction Type                                                 | March | April | May  | June | July | August | September | October | % Distribution |
|------------------------------------------------------------------|-------|-------|------|------|------|--------|-----------|---------|----------------|
| Money transfer from a debit card on their Kowri account to a mobile money subscriber (Type A) | 350   | 450   | 896  | 940  | 1200 | 3400   | 4400      | 6456    | 59.50%         |
| Money transfer from a debit card on their Kowri account to a recipient’s bank account (Type B) | 100   | 120   | 80   | 460  | 960  | 2200   | 1345      | 2178    | 24.48%         |
| Money transfer from a mobile money wallet added to Kowri to a bank account (Type C)           | 75    | 72    | 100  | 315  | 875  | 670    | 892       | 592     | 11.81%         |
| Money transfer from a mobile money wallet added on Kowri to another mobile money wallet (Type D) | 20    | 45    | 48   | 124  | 389  | 230    | 197       | 226     | 4.21%          |

### Transaction Fees

| Transaction Type                                      | Transactions above $84 | Transactions below $84 |
|-------------------------------------------------------|------------------------|------------------------|
| Send Money from Linked Card to mobile money           | $0.83                  | 1%                     |
| Send Money from Linked Card to bank                   | 1%                     | 1%                     |
| Send Money from linked mobile money to a mobile money wallet | $0.83                  | 1%                     |
| Send Money from linked mobile money to a bank account | 1%                     | 1%                     |

## Monthly Fees

- **App development**: Handled by an in-house team of six developers, using Agile methodology with 2-week sprints.
- **Estimated Cost**: $40 an hour (average market rate), resulting in $240 an hour for the team. The total cost for a full 2-week sprint (80 hours) is approximately $19,200 per sprint.
- **Note**: Actual costs are lower due to Ghana's relatively lower rates.

## Mathematical Model

### Inputs

- **i**: Index for the transaction type \( i \in \{1, 2, 3, 4\} \)
- **TV_i**: Average transaction amount per user for transaction type \( i \)
- **I_i**: Integration fees for transaction type \( i \)
- **P_i**: Percentage of transactions for transaction type \( i \)
- **A**: Average number of transactions per user
- **U**: Number of current active users
- **C**: Customer acquisition cost (=$2)
- **F**: Fixed overhead costs ($208,800)
- **CC_i**: Closest competition transaction rates for type \( i \)

### Decision Variables

- **TR_i**: Transaction rate to charge customers for transaction type \( i \)
- **N**: Number of customers to acquire into user base

### Objective Function

\[ \max_{TR_i, N} \sum_{j \in \{1, 2\}} (TR_i - I_i) \times (U + N) \times A \times P_i \times TV_i - (C \times N) - F \]

### Constraints

- \( TR_i \leq CC_i \quad \forall i \in \{1, 2, 3, 4\} \)
- \( TR_i \geq 0 \)
- \( N \geq 0 \)

## Conclusion

Sevn needs to negotiate better transaction fees with the integrators. As customer usage of Kowri increases, so do the operating costs.

---

For more details on the Kowri app, visit [www.kowri.app](http://www.kowri.app).
