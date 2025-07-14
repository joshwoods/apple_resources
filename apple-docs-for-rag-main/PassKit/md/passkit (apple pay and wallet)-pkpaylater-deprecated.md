

- PassKit (Apple Pay and Wallet)
-  PKPayLater Deprecated

Enumeration

# PKPayLater

Functions for validating information the framework displays in an Apple Pay Later visual merchandising widget.

iOS 17.0+iPadOS 17.0+visionOS

``` source
@frozen
enum PKPayLater
```

Deprecated

Apple Pay Later is deprecated.

## Topics

### Utilities

static func validate(amount: Decimal, currency: Locale.Currency) async -> Bool

Checks if the framework can display Apple Pay Later visual merchandising widget information for the given amount and currency.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

