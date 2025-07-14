

- SwiftUI
-  TransactionKey 

Protocol

# TransactionKey

A key for accessing values in a transaction.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol TransactionKey
```

## Overview

You can create custom transaction values by extending the Transaction structure with new properties. First declare a new transaction key type and specify a value for the required defaultValue property:

```
private struct MyTransactionKey: TransactionKey {
    static let defaultValue = false
}
```

The Swift compiler automatically infers the associated Value type as the type you specify for the default value. Then use the key to define a new transaction value property:

```
extension Transaction {
    var myCustomValue: Bool {
        get { self[MyTransactionKey.self] }
        set { self[MyTransactionKey.self] = newValue }
    }
}
```

Clients of your transaction value never use the key directly. Instead, they use the key path of your custom transaction value property. To set the transaction value for a change, wrap that change in a call to `withTransaction`:

```
withTransaction(\.myCustomValue, true) {
    isActive.toggle()
}
```

To use the value from inside `MyView` or one of its descendants, use the transaction(_:) view modifier:

```
MyView()
    .transaction { transaction in
        if transaction.myCustomValue {
            transaction.animation = .default.repeatCount(3)
        }
    }
```

## Topics

### Setting a default value

static var defaultValue: Self.Value

The default value for the transaction key.

**Required**

associatedtype Value

The associated type representing the type of the transaction key’s value.

**Required**

## See Also

### Moving an animation to another view

func withTransaction&lt;Result>(Transaction, () throws -> Result) rethrows -> Result

Executes a closure with the specified transaction and returns the result.

func withTransaction&lt;R, V>(WritableKeyPath&lt;Transaction, V>, V, () throws -> R) rethrows -> R

Executes a closure with the specified transaction key path and value and returns the result.

func transaction((inout Transaction) -> Void) -> some View

Applies the given transaction mutation function to all animations used within the view.

func transaction(value: some Equatable, (inout Transaction) -> Void) -> some View

Applies the given transaction mutation function to all animations used within the view.

func transaction&lt;V>((inout Transaction) -> Void, body: (PlaceholderContentView&lt;Self>) -> V) -> some View

Applies the given transaction mutation function to all animations used within the `body` closure.

struct Transaction

The context of the current state-processing update.

macro Entry()

Creates an environment values, transaction, container values, or focused values entry.

