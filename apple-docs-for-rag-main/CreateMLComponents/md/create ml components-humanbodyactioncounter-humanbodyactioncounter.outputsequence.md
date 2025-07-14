

- Create ML Components
- HumanBodyActionCounter
-  HumanBodyActionCounter.OutputSequence 

Type Alias

# HumanBodyActionCounter.OutputSequence

The output async sequence type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias OutputSequence = HumanBodyActionCounter.CumulativeSumSequence
```

## See Also

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> HumanBodyActionCounter.OutputSequence

Predicts cumulative human body action counts from a sequence of human body pose windows.

typealias Input

The input type.

typealias Output

The output type.

struct CumulativeSumSequence

Cumulative human body action count sequence.

