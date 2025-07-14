

- PassKit (Apple Pay and Wallet)
- Apple Pay
-  Complying with regional regulations 

Article

# Complying with regional regulations

Check regional regulations for possible requirements for your Apple Pay-based implementation.

## Overview

Some regional regulations may require specific configurations in your Apple Pay implementation, such as including certain options in properties. Below is some guidance on configuring your implementation in current Apple Pay markets.

Note

This list may not be complete. Check with your payment service provider (PSP) or the appropriate authorities to ensure your implementation meets requirements.

United Kingdom and European Economic Area  
Transactions that take place in the United Kingdom and European Economic Area may be subject to The Payment Services Directive 2 (PSD2). Set the `countryCode` of the transaction to the region where it’s processed. Apple Pay uses the `countryCode` to generate data for the transaction that complies with this regulation.

You’re also required to show a final amount on the payment sheet.

For more information on PSD2, see Strong Customer Authentication Transactions in the European Economic Area.

Saudi Arabia  
Saudi Arabia requires that all domestic debit transactions use the mada network. Merchants based in Saudi Arabia that support debit cards should add the mada payment network to their supported payment networks. If merchants don’t include mada, Apple Pay users may not be able to use certain Saudi-issued cards when the `countryCode` is `SA` (Saudi Arabia). Merchants using a PSP should confirm they support the mada network.

## See Also

### Apple Pay setup

Setting up Apple Pay

Fulfill the requirements to provide Apple Pay as a payment option on your website or in your app.

Offering Apple Pay in Your App

Collect payments with iPhone and Apple Watch using Apple Pay.

