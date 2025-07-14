

- Create ML Components
- ComposedTemporalTransformer
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs the composed transformation on an input sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: S,
    eventHandler: EventHandler? = nil
) async throws -> ComposedTemporalTransformer.OutputSequence where S : TemporalSequence, Inner.Input == S.Feature
```

## Parameters 

`input`  

The input temporal sequence.

`eventHandler`  

An event handler.

## Return Value

An async sequence produced by applying the transformation to the input.

## See Also

### Applying a transformer

typealias Intermediate

The intermediate type.

typealias Input

The input type.

typealias Output

The output type.

typealias OutputSequence

The output sequence type.

