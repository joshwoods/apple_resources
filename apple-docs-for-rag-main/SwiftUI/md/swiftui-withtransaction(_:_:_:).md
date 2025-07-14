

- SwiftUI
-  withTransaction(\_:\_:\_:) 

Function

# withTransaction(\_:\_:\_:)

Executes a closure with the specified transaction key path and value and returns the result.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withTransaction(
    _ keyPath: WritableKeyPath,
    _ value: V,
    _ body: () throws -> R
) rethrows -> R
```

## Parameters 

`keyPath`  

A key path that indicates the property of the Transaction structure to update.

`value`  

The new value to set for the item specified by `keyPath`.

`body`  

A closure to execute.

## Return Value

The result of executing the closure with the specified transaction value.

## See Also

### Moving an animation to another view

func withTransaction&lt;Result>(Transaction, () throws -> Result) rethrows -> Result

Executes a closure with the specified transaction and returns the result.

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

protocol TransactionKey

A key for accessing values in a transaction.

