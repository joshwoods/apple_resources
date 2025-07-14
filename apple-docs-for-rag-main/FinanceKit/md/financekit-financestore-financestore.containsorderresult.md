

- FinanceKit
- FinanceStore
-  FinanceStore.ContainsOrderResult 

Enumeration

# FinanceStore.ContainsOrderResult

Result type for queries against the finance store’s orders.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum ContainsOrderResult
```

## Overview

These values represent the possible results of the `containsOrder` method you use to check whether an order you specified exists in the `FinanceStore`.

## Topics

### Operators

static func == (FinanceStore.ContainsOrderResult, FinanceStore.ContainsOrderResult) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case exists

The specified order exists.

case newerExists

A newer order than the one you specified exists.

case notFound

The specified order doesn’t exist.

case olderExists

A older order than the one you specified exists.

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

static var allCases: [FinanceStore.ContainsOrderResult]

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

enum DataType

Values that describe the kinds of data in the finance store.

enum SaveOrderResult

Result type for the finance store’s save order method.

