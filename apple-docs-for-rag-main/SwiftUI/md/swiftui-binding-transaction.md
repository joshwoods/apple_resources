

- SwiftUI
- Binding
-  transaction 

Instance Property

# transaction

The binding’s transaction.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var transaction: Transaction
```

## Discussion

The transaction captures the information needed to update the view when the binding value changes.

## See Also

### Managing changes

var id: Value.ID

The stable identity of the entity associated with this instance, corresponding to the `id` of the binding’s wrapped value.

func animation(Animation?) -> Binding&lt;Value>

Specifies an animation to perform when the binding value changes.

func transaction(Transaction) -> Binding&lt;Value>

Specifies a transaction for the binding.

