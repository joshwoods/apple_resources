

- PassKit (Apple Pay and Wallet)
- PKStoredValuePassBalance
-  amount 

Instance Property

# amount

The current balance of a stored-value pass in money or points.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOSwatchOS 8.0+

``` source
var amount: Decimal { get }
```

## See Also

### Getting the pass status

var expiryDate: Date?

The date that the balance expires.

var balanceType: PKStoredValuePassBalance.BalanceType

The type of value that the balance represents, such as money or points.

var currencyCode: String?

The ISO 4217 currency code of the balance.

struct BalanceType

The type of value that the balance represents, such as money or points.

