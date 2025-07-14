

- App Intents
- IntentCurrencyAmount
-  init(amount:currencyCode:) 

Initializer

# init(amount:currencyCode:)

Creates a IntentCurrencyAmount from a monetary amount and a currency code.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    amount: Decimal,
    currencyCode: String
)
```

## Parameters 

`amount`  

Monetary amount

`currencyCode`  

ISO 4217 currency code that applies to the monetary amount.

