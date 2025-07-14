

- Create ML Components
- HumanBodyActionCounter
-  HumanBodyActionCounter.Input 

Type Alias

# HumanBodyActionCounter.Input

The input type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias Input = [Pose]
```

## See Also

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> HumanBodyActionCounter.OutputSequence

Predicts cumulative human body action counts from a sequence of human body pose windows.

typealias Output

The output type.

struct CumulativeSumSequence

Cumulative human body action count sequence.

typealias OutputSequence

The output async sequence type.

