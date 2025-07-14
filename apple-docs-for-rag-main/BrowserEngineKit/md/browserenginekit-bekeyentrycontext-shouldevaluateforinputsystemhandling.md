

- BrowserEngineKit
- BEKeyEntryContext
-  shouldEvaluateForInputSystemHandling 

Instance Property

# shouldEvaluateForInputSystemHandling

Represents whether the key event should be evaluated within the context of a composed input mode.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var shouldEvaluateForInputSystemHandling: Bool { get set }
```

## Discussion

When using an input mode with composed input, such as Chinese/Japanese/Korean, the markedText will be used to combine multiple key events into a single character.

## See Also

### Getting the information about the key event

var keyEntry: BEKeyEntry

BEKeyEntry for which this context is representing.

var shouldInsertCharacter: Bool

Represents whether a character should be inserted.

