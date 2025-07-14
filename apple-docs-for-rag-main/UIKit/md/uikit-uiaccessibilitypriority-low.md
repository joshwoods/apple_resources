

- UIKit
- UIAccessibilityPriority
-  low 

Type Property

# low

A low-priority announcement that the system queues and speaks after other speech utterances are complete.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
static let low: UIAccessibilityPriority
```

## See Also

### Choosing a priority

static let high: UIAccessibilityPriority

A high-priority announcement that interrupts other speech and isn’t interruptible after it starts.

static let `default`: UIAccessibilityPriority

A default-priority announcement that interrupts existing speech, but is interruptible if a new speech utterance starts.

