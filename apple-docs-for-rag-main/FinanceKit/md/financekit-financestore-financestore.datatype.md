

- FinanceKit
- FinanceStore
-  FinanceStore.DataType 

Enumeration

# FinanceStore.DataType

Values that describe the kinds of data in the finance store.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum DataType
```

## Topics

### Operators

static func == (FinanceStore.DataType, FinanceStore.DataType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case financialData

The value that describes financial data, such as account information.

case orders

The value that describes orders records, such as purchases.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Enumerations

enum ContainsOrderResult

Result type for queries against the finance store’s orders.

enum SaveOrderResult

Result type for the finance store’s save order method.

