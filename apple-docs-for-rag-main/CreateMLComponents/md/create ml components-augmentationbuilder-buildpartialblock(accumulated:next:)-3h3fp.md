

- Create ML Components
- AugmentationBuilder
-  buildPartialBlock(accumulated:next:) 

Type Method

# buildPartialBlock(accumulated:next:)

Builds a partial result by combining an accumulated random transformer and a new random transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
static func buildPartialBlock(
    accumulated: some RandomTransformer,
    next: some RandomTransformer
) -> some RandomTransformer
```

## Parameters 

`accumulated`  

A random transformer representing the accumulated result thus far.

`next`  

A random transformer representing the next component after the accumulated ones in the block.

## See Also

### Building augmentations

static func buildPartialBlock(accumulated: some RandomTransformer&lt;Element, Element>, next: some Transformer&lt;Element, Element>) -> some RandomTransformer&lt;Element, Element> 

Builds a partial result by combining an accumulated random transformer and a new transformer.

static func buildPartialBlock(first: some RandomTransformer&lt;Element, Element>) -> some RandomTransformer&lt;Element, Element> 

Builds a partial result random transformer from the first random transformer.

static func buildPartialBlock(first: some Transformer&lt;Element, Element>) -> some RandomTransformer&lt;Element, Element> 

Builds a partial result from the first transformer.

