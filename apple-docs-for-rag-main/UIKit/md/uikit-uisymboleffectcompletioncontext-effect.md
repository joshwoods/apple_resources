

- UIKit
- UISymbolEffectCompletionContext
-  effect 

Instance Property

# effect

The symbol effect that completed.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor
var effect: any SymbolEffect { get }
```

## Discussion

For a symbol effect completion, this property may not be the same instance as the original effect.

For a content transition completion, this property is `nil.`

## See Also

### Determining completion status

var isFinished: Bool

A Boolean value that indicates whether the symbol effect finished completely.

var sender: AnyObject?

The object, an image view or bar button item, that received the symbol effect.

