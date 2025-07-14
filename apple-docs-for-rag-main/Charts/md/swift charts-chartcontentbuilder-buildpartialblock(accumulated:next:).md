

- Swift Charts
- ChartContentBuilder
-  buildPartialBlock(accumulated:next:) 

Type Method

# buildPartialBlock(accumulated:next:)

Builds a partial result by combining an accumulated component and a new component.

``` source
static func buildPartialBlock(
    accumulated: some ChartContent,
    next: some ChartContent
) -> some ChartContent
```

## Parameters 

`accumulated`  

The accumulated result.

`next`  

The next component to accumulate.

## See Also

### Building chart content

static func buildPartialBlock&lt;T>(first: T) -> T

Builds a partial result from a single, first component.

Deprecated

static func buildBlock() -> some ChartContent

Produces empty chart content.

