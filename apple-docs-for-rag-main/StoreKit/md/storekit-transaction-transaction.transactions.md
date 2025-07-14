

- StoreKit
- Transaction
-  Transaction.Transactions 

Structure

# Transaction.Transactions

An asynchronous sequence of transactions.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Transactions
```

## Overview

You don’t create a Transaction.Transactions sequence directly. Use methods such as all, updates, or currentEntitlements to get transactions.

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Monitoring transaction-related changes

static var updates: Transaction.Transactions

The asynchronous sequence that emits a transaction when the system creates or updates transactions that occur outside the app or on other devices.

