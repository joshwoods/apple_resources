

- Create ML Components
- ComposedTransformer
-  ComposedTransformer.Input 

Type Alias

# ComposedTransformer.Input

The input type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Input = Inner.Input
```

## See Also

### Performing the transformation

func applied(to: ComposedTransformer&lt;Inner, Outer>.Input, eventHandler: EventHandler?) async throws -> ComposedTransformer&lt;Inner, Outer>.Output

Performs the composed transformation on a single input.

typealias Intermediate

The intermediate type.

typealias Output

The output type.

