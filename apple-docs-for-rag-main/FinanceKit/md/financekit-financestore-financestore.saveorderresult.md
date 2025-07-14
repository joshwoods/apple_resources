

- FinanceKit
- FinanceStore
-  FinanceStore.SaveOrderResult 

Enumeration

# FinanceStore.SaveOrderResult

Result type for the finance store’s save order method.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum SaveOrderResult
```

## Topics

### Operators

static func == (FinanceStore.SaveOrderResult, FinanceStore.SaveOrderResult) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case added

The framework added the order to the finance store.

case cancelled

The individual canceled the order.

case newerExisting

There’s a newer, existing order already in the finance store.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

### Type Properties

static var allCases: [FinanceStore.SaveOrderResult]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Equatable
- Hashable
- Sendable

## See Also

### Enumerations

enum ContainsOrderResult

Result type for queries against the finance store’s orders.

enum DataType

Values that describe the kinds of data in the finance store.

