

- Create ML Components
- HumanBodyActionCounter
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Predicts cumulative human body action counts from a sequence of human body pose windows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to input: S,
    eventHandler: EventHandler? = nil
) async throws -> HumanBodyActionCounter.OutputSequence where S : TemporalSequence, S.Feature == [Pose]
```

## Parameters 

`input`  

An async sequence of human body pose windows.

`eventHandler`  

An event handler.

## Return Value

An async sequence of cumulative human body action counts.

## See Also

### Performing the transformation

typealias Input

The input type.

typealias Output

The output type.

struct CumulativeSumSequence

Cumulative human body action count sequence.

typealias OutputSequence

The output async sequence type.

