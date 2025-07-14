

- UIKit
- UIConfigurationTextAttributesTransformer
-  callAsFunction(\_:) 

Instance Method

# callAsFunction(\_:)

Calls the transform closure of the text attributes transformer.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
func callAsFunction(_ input: AttributeContainer) -> AttributeContainer
```

## Parameters 

`input`  

The current attributes container for a string.

## Return Value

A new, transformed attributes container.

## Discussion

Using this syntax, you can call the text attributes transformer type as if it were a closure:

```
var container = AttributeContainer()
container.backgroundColor = UIColor.blue
let transformer = UIConfigurationTextAttributesTransformer { incoming in
    var outgoing = incoming
    outgoing.backgroundColor = incoming.backgroundColor?.withAlphaComponent(0.6)
    return outgoing
}
let transformed = transformer.callAsFunction(container)

```

