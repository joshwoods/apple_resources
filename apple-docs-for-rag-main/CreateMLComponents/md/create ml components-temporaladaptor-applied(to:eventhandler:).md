

- Create ML Components
- TemporalAdaptor
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs the transformation on each element of the input sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func applied(
    to input: some TemporalSequence,
    eventHandler: EventHandler? = nil
) async throws -> AnyTemporalSequence.Output>
```

