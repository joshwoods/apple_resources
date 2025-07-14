

- PassKit (Apple Pay and Wallet)
- PKStoredValuePassBalance
-  PKStoredValuePassBalance.BalanceType 

Structure

# PKStoredValuePassBalance.BalanceType

The type of value that the balance represents, such as money or points.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct BalanceType
```

## Topics

### Creating a balance type

init(rawValue: String)

Creates a balance type.

### Reading the balance type

static let cash: PKStoredValuePassBalance.BalanceType

An identifier indicating a balance that represents money.

static let loyaltyPoints: PKStoredValuePassBalance.BalanceType

An identifier indicating a balance that represents points.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the pass status

var expiryDate: Date?

The date that the balance expires.

var amount: Decimal

The current balance of a stored-value pass in money or points.

var balanceType: PKStoredValuePassBalance.BalanceType

The type of value that the balance represents, such as money or points.

var currencyCode: String?

The ISO 4217 currency code of the balance.

