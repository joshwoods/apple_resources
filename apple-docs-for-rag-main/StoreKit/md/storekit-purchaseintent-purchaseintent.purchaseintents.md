

- StoreKit
- PurchaseIntent
-  PurchaseIntent.PurchaseIntents 

Structure

# PurchaseIntent.PurchaseIntents

An asynchronous sequence of purchase intents for purchases that customers initiate outside of the app.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 14.4+

``` source
struct PurchaseIntents
```

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Getting purchase intents

static var intents: PurchaseIntent.PurchaseIntents

The asynchronous sequence that emits a purchase intent when customers initiate a purchase outside of the app.

