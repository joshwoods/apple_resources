

- Create ML Components
- TemporalAdaptor
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs the transformation on a sequence of annotated input sequences.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: S,
    eventHandler: EventHandler? = nil
) async throws -> [AnnotatedFeature] where S : Sequence, TS : TemporalSequence, Self.Input == TS.Feature, S.Element == AnnotatedFeature
```

## Parameters 

`input`  

A sequence of annotated sequences.

`eventHandler`  

An event handler.

## Return Value

The annotated outputs produced by applying the transformer to the inputs.

