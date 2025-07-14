

- Create ML Components
- AugmentationBuilder
-  buildPartialBlock(first:) 

Type Method

# buildPartialBlock(first:)

Builds a partial result from the first transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
static func buildPartialBlock(first: some Transformer) -> some RandomTransformer
```

## Parameters 

`first`  

A transformer.

## See Also

### Building augmentations

static func buildPartialBlock(accumulated: some RandomTransformer&lt;Element, Element>, next: some RandomTransformer&lt;Element, Element>) -> some RandomTransformer&lt;Element, Element> 

Builds a partial result by combining an accumulated random transformer and a new random transformer.

static func buildPartialBlock(accumulated: some RandomTransformer&lt;Element, Element>, next: some Transformer&lt;Element, Element>) -> some RandomTransformer&lt;Element, Element> 

Builds a partial result by combining an accumulated random transformer and a new transformer.

static func buildPartialBlock(first: some RandomTransformer&lt;Element, Element>) -> some RandomTransformer&lt;Element, Element> 

Builds a partial result random transformer from the first random transformer.

