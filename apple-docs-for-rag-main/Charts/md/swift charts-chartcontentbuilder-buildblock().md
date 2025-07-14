

- Swift Charts
- ChartContentBuilder
-  buildBlock() 

Type Method

# buildBlock()

Produces empty chart content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildBlock() -> some ChartContent
```

## See Also

### Building chart content

static func buildPartialBlock&lt;T>(first: T) -> T

Builds a partial result from a single, first component.

Deprecated

static func buildPartialBlock(accumulated: some ChartContent, next: some ChartContent) -> some ChartContent

Builds a partial result by combining an accumulated component and a new component.

Deprecated

