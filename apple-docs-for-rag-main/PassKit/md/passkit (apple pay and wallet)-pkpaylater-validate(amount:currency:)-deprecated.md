

- PassKit (Apple Pay and Wallet)
- PKPayLater
-  validate(amount:currency:) Deprecated

Type Method

# validate(amount:currency:)

Checks if the framework can display Apple Pay Later visual merchandising widget information for the given amount and currency.

iOS 17.0+iPadOS 17.0+visionOS

``` source
static func validate(
    amount: Decimal,
    currency: Locale.Currency
) async -> Bool
```

Deprecated

Apple Pay Later is deprecated.

## Parameters 

`amount`  

The customer’s cart price or item pricing.

`currency`  

The ISO-4217 currency code for the country or region of the merchant’s principle place of business.

## Return Value

Returns true if the framework can display the requested information; otherwise, false.

