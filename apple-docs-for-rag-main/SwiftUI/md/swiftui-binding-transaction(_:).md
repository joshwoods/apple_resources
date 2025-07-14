

- SwiftUI
- Binding
-  transaction(\_:) 

Instance Method

# transaction(\_:)

Specifies a transaction for the binding.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func transaction(_ transaction: Transaction) -> Binding
```

## Return Value

A new binding.

## See Also

### Managing changes

var id: Value.ID

The stable identity of the entity associated with this instance, corresponding to the `id` of the binding’s wrapped value.

func animation(Animation?) -> Binding&lt;Value>

Specifies an animation to perform when the binding value changes.

var transaction: Transaction

The binding’s transaction.

