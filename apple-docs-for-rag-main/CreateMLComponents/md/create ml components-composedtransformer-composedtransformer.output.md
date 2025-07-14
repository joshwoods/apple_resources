

- Create ML Components
- ComposedTransformer
-  ComposedTransformer.Output 

Type Alias

# ComposedTransformer.Output

The output type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Output = Outer.Output
```

## See Also

### Performing the transformation

func applied(to: ComposedTransformer&lt;Inner, Outer>.Input, eventHandler: EventHandler?) async throws -> ComposedTransformer&lt;Inner, Outer>.Output

Performs the composed transformation on a single input.

typealias Input

The input type.

typealias Intermediate

The intermediate type.

