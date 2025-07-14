

- PassKit (Apple Pay and Wallet)
- PKStoredValuePassBalance
-  balanceType 

Instance Property

# balanceType

The type of value that the balance represents, such as money or points.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSvisionOS 1.0+watchOS 8.0+

``` source
var balanceType: PKStoredValuePassBalance.BalanceType { get }
```

## See Also

### Getting the pass status

var expiryDate: Date?

The date that the balance expires.

var amount: Decimal

The current balance of a stored-value pass in money or points.

var currencyCode: String?

The ISO 4217 currency code of the balance.

struct BalanceType

The type of value that the balance represents, such as money or points.

