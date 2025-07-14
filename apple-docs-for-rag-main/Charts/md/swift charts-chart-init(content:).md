

- Swift Charts
- Chart
-  init(content:) 

Initializer

# init(content:)

Creates a chart composed of any number of data series and individual marks.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(@ChartContentBuilder content: () -> Content)
```

## Parameters 

`content`  

A chart content builder that returns the marks that the chart should draw.

## Discussion

This initializer draws the marks that you specify in the `content` input. You can provide individual marks, or marks produced by one or more ForEach constructs, or any combination of these. As a convenience when you have exactly one `ForEach` in your chart’s content, you can use either the init(_:content:) or init(_:id:content:) initializer instead, either of which wraps the content in an implicit `ForEach`.

## See Also

### Creating a chart

init&lt;Data, C>(Data, content: (Data.Element) -> C)

Creates a chart composed of a series of identifiable marks.

init&lt;Data, ID, C>(Data, id: KeyPath&lt;Data.Element, ID>, content: (Data.Element) -> C)

Creates a chart composed of a series of marks.

