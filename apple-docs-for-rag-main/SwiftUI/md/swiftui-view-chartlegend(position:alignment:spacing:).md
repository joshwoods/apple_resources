

- SwiftUI
- View
-  chartLegend(position:alignment:spacing:) 

Instance Method

# chartLegend(position:alignment:spacing:)

Configures the legend for charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
func chartLegend(
    position: AnnotationPosition = .automatic,
    alignment: Alignment? = nil,
    spacing: CGFloat? = nil
) -> some View
```

## Parameters 

`position`  

Configures the position of the legend.

`alignment`  

Alignment of the legend within the space available to it. Use `nil` for default alignment.

`spacing`  

Distance between the legend and the chart. Use `nil` for the default spacing.

## See Also

### Legends

func chartLegend(Visibility) -> some View

Configures the legend for charts.

func chartLegend&lt;Content>(position: AnnotationPosition, alignment: Alignment?, spacing: CGFloat?, content: () -> Content) -> some View

Configures the legend for charts.

