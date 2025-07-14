

- UIKit
- UISymbolEffectCompletionContext
-  sender 

Instance Property

# sender

The object, an image view or bar button item, that received the symbol effect.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor
weak var sender: AnyObject? { get }
```

## See Also

### Determining completion status

var effect: any SymbolEffect

The symbol effect that completed.

var isFinished: Bool

A Boolean value that indicates whether the symbol effect finished completely.

