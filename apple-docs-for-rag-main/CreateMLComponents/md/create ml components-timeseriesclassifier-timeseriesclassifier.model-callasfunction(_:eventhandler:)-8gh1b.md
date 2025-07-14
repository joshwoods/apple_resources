

- Create ML Components
- TimeSeriesClassifier
- TimeSeriesClassifier.Model
-  callAsFunction(\_:eventHandler:) 

Instance Method

# callAsFunction(\_:eventHandler:)

Performs the transformation on an input sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func callAsFunction(
    _ input: S,
    eventHandler: EventHandler? = nil
) async throws -> Self.OutputSequence where S : TemporalSequence, Self.Input == S.Feature
```

## Parameters 

`input`  

The input temporal sequence.

`eventHandler`  

An event handler.

## Return Value

An async sequence produced by applying the transformation to the input.

