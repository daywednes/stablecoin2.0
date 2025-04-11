# Stablecoins 2.0 Research Notes

## Academic Paper: "Stablecoins 2.0: Economic Foundations and Risk-based Models"

### Authors
- Ariah Klages-Mundt (Cornell University)
- Dominik Harz (Imperial College London)
- Lewis Gudgeon (Imperial College London)
- Jun-You Liu (Cornell University)
- Andreea Minca (Cornell University)

### Key Insights (From Pages 1-2)

#### Abstract
- Stablecoins are one of the most widely capitalized types of cryptocurrency
- Their risks vary significantly according to design and are often poorly understood
- The paper aims to provide a sound foundation for stablecoin theory with risk-based functional characterization
- The authors characterize unique risks in non-custodial stablecoins and develop a model framework

#### Introduction
- Stablecoins are cryptocurrencies with an added economic structure aiming to stabilize price and purchasing power
- Two main classes: 
  1. Custodial stablecoins (require trust in a third party)
  2. Non-custodial stablecoins (replace trust with economic mechanisms)
- Major custodial examples: Tether, Binance USD, USDC, TrueUSD (combined market cap over $150 billion)
- Non-custodial side: Over 50% of value locked in DeFi protocols allocated to Maker's Dai stablecoin

#### Risk Dimensions
The paper identifies five central dimensions of risks in non-custodial stablecoins:
1. Effects from deleveraging-like processes on collateral-like assets
2. Data feed and governance risks
3. Base layer risks from mining incentives
4. Smart contract coding risks
5. Censorship and counterparty risk (applies differently in custodial stablecoins)

#### Stablecoin Types
1. **Reserve Fund Stablecoins**
   - Resemble e-money, narrow banks, and currency boards
   - Backed by 100% reserves at a central bank
   - Example: Hong Kong Dollar maintains USD peg using USD reserves

2. **Fractional Reserve Fund**
   - Backed by mixture of reserve assets and other capital assets
   - Has a target price
   - Holds reserves in target asset (or highly liquid stable assets)
   - Reserve assets may resemble commercial bank deposits
   - Other capital assets account for remaining stablecoin supply value

#### Contributions
- Functional breakdown of custodial stablecoin designs with taxonomy and models
- Common functional framework for non-custodial stablecoin designs
- Questions of economic stability and security for non-custodial stablecoins
- Framework of models for measuring stability and security
- Methods for estimating agents' preferences
- Application to DeFi protocols including composite stablecoins and cross-chain systems

# Stablecoins 2.0 Research Notes

## Academic Paper: "Stablecoins 2.0: Economic Foundations and Risk-based Models"

### Authors
- Ariah Klages-Mundt (Cornell University)
- Dominik Harz (Imperial College London)
- Lewis Gudgeon (Imperial College London)
- Jun-You Liu (Cornell University)
- Andreea Minca (Cornell University)

### Key Insights (From Pages 1-2)

#### Abstract
- Stablecoins are one of the most widely capitalized types of cryptocurrency
- Their risks vary significantly according to design and are often poorly understood
- The paper aims to provide a sound foundation for stablecoin theory with risk-based functional characterization
- The authors characterize unique risks in non-custodial stablecoins and develop a model framework

#### Introduction
- Stablecoins are cryptocurrencies with an added economic structure aiming to stabilize price and purchasing power
- Two main classes: 
  1. Custodial stablecoins (require trust in a third party)
  2. Non-custodial stablecoins (replace trust with economic mechanisms)
- Major custodial examples: Tether, Binance USD, USDC, TrueUSD (combined market cap over $150 billion)
- Non-custodial side: Over 50% of value locked in DeFi protocols allocated to Maker's Dai stablecoin

#### Risk Dimensions
The paper identifies five central dimensions of risks in non-custodial stablecoins:
1. Effects from deleveraging-like processes on collateral-like assets
2. Data feed and governance risks
3. Base layer risks from mining incentives
4. Smart contract coding risks
5. Censorship and counterparty risk (applies differently in custodial stablecoins)

### Stablecoin Types and Mechanisms (Pages 2-6)

#### Custodial Stablecoins
1. **Reserve Fund Stablecoins**
   - Resemble e-money, narrow banks, and currency boards
   - Backed by 100% reserves at a central bank
   - Example: Hong Kong Dollar maintains USD peg using USD reserves
   - Stablecoin maintains 1:1 reserve ratio
   - Price target maintained via two mechanisms:
     - Direct redemption for underlying asset
     - Arbitrage by external actors

2. **Fractional Reserve Fund**
   - Backed by mixture of reserve assets and other capital assets
   - Has a target price
   - Holds reserves in target asset (or highly liquid stable assets)
   - Reserve assets may resemble commercial bank deposits
   - Other capital assets account for remaining stablecoin supply value
   - Subject to price risk with important dividing point being capital assets held

3. **Central Bank Digital Currency (CBDC)**
   - Consumer-facing fiat digital currency providing risk-free store of value
   - Different monetary system from status quo
   - Central bank deposits available to commercial banks but not consumers
   - CBDC represents change in banking system structure and currency stability model
   - More ideal setting for existing currency models than fiat

#### Non-Custodial Stablecoins
- Aim to be independent of societal institutions that custodial designs rely on
- Achieve this by establishing economic structure through smart contracts
- Structurally resemble dynamic versions of risk transfer instruments
- Collateralized debt obligations (CDOs) and contracts for difference (CFDs)
- Backed by collateral assets sliced into tranches

#### Components of Non-Custodial Stablecoins
1. **Primary Value**
   - Economic structure of base value in the stablecoin system
   - Abstracted concept of collateral with types:
     - **Exogenous collateral**: Asset with uses outside stablecoin system (e.g., ETH in Maker)
     - **Endogenous collateral**: Asset created for purpose of being collateral (e.g., SNX in Synthetix)
     - **Implicit collateral**: No explicit market prices, coordinated confidence in system

2. **Risk Absorbers**
   - Speculative agents who absorb risk and profit in the system
   - Represent junior tranche of a CDO

3. **Stablecoin Holders**
   - Agents who make up demand side of stablecoin market
   - Represent senior tranche holder of a CDO

4. **Issuance**
   - Function determining stablecoin issuance
   - Includes deleveraging process to reduce supply
   - Two general types:
     - **Agent-based issuance**: Size of supply decided by agents optimizing positions
     - **Algorithmic issuance**: Process to adjust leverage codified in protocol

5. **Governance**
   - Function to manage system parameters
   - Manages deleveraging factors and price feeds
   - Collects fees on system operation

### Risk Absorption and Issuance (Pages 5-6)
- Stablecoin mechanism works when speculators incentivized to absorb price risk
- Two primary forms:
  1. **Equity risk absorption**: Secondary asset exists, holders implicitly absorb risk
  2. **Agent risk absorption**: Individual agents manage vaults containing primary value

### Governance, Mining, and Manipulation (Page 6)
- Design components that introduce manipulation potential
- In custodial systems, manipulations avoided by societal institutions
- Permissionless systems lack strong identities, opening anonymous attack vectors
- **Data Feeds**: Non-custodial stablecoins require asset price data for target peg
- **Governance**: Tasked with managing system parameters (interest rates, collateral factors)
- **Miners**: Maintain blockchain, decide transaction inclusion and ordering

### Key Challenges and Innovations
- Deleveraging risks in leveraged lending markets
- Feedback effects on stablecoin market and collateral value
- Insurance mechanisms to mitigate risk
- Buffer designs to extend stability regions
- Data feed manipulation risks
- Governance attacks and system stability
