

- PassKit (Apple Pay and Wallet)
- PKPayLaterView
-  init(amount:currency:) Deprecated

Initializer

# init(amount:currency:)

Creates a new Apple Pay Later visual merchandising widget view with the shopping cart amount and currency you specify.

iOS 17.0+iPadOS 17.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    amount: Decimal,
    currency: Locale.Currency
)
```

Deprecated

Apple Pay Later is deprecated.

## Parameters 

`amount`  

The customer’s shopping cart or item pricing.

`currency`  

The ISO-4217 currency code for the country or region of the merchant’s principle place of business.

