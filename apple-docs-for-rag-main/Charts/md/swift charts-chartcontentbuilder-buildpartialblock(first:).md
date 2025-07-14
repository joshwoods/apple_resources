

- Swift Charts
- ChartContentBuilder
-  buildPartialBlock(first:) 

Type Method

# buildPartialBlock(first:)

Builds a partial result from a single, first component.

``` source
static func buildPartialBlock(first content: T) -> T where T : ChartContent
```

## Parameters 

`content`  

The first component to accumulate.

## See Also

### Building chart content

static func buildPartialBlock(accumulated: some ChartContent, next: some ChartContent) -> some ChartContent

Builds a partial result by combining an accumulated component and a new component.

Deprecated

static func buildBlock() -> some ChartContent

Produces empty chart content.

