

- Create ML Components
- ComposedTemporalTransformer
-  ComposedTemporalTransformer.Intermediate 

Type Alias

# ComposedTemporalTransformer.Intermediate

The intermediate type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Intermediate = Inner.Output
```

## See Also

### Applying a transformer

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> ComposedTemporalTransformer&lt;Inner, Outer>.OutputSequence

Performs the composed transformation on an input sequence.

typealias Input

The input type.

typealias Output

The output type.

typealias OutputSequence

The output sequence type.

