

- SwiftUI
- Binding
-  animation(\_:) 

Instance Method

# animation(\_:)

Specifies an animation to perform when the binding value changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func animation(_ animation: Animation? = .default) -> Binding
```

## Parameters 

`animation`  

An animation sequence performed when the binding value changes.

## Return Value

A new binding.

## See Also

### Managing changes

var id: Value.ID

The stable identity of the entity associated with this instance, corresponding to the `id` of the binding’s wrapped value.

func transaction(Transaction) -> Binding&lt;Value>

Specifies a transaction for the binding.

var transaction: Transaction

The binding’s transaction.

