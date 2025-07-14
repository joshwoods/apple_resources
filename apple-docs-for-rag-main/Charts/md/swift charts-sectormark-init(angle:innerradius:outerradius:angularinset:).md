

- Swift Charts
- SectorMark
-  init(angle:innerRadius:outerRadius:angularInset:) 

Initializer

# init(angle:innerRadius:outerRadius:angularInset:)

Creates a sector mark, which uses the angular size to represent the proportion of the value to the sum of all values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    angle: PlottableValue,
    innerRadius: MarkDimension = .automatic,
    outerRadius: MarkDimension = .automatic,
    angularInset: CGFloat? = nil
)
```

## Parameters 

`angle`  

A plottable value that will map to the angular size of the sector. It’s either a value that the angle within the full circle will be proportional with, or a value range for explicit start/end angles.

`innerRadius`  

The inner radius of the sector. It is either a size in points, or a `.ratio` or `.inset` relative to the outer radius.

`outerRadius`  

The outer radius of the sector. It is either a size in points, or a `.ratio`or `.inset` relative to the available plot area.

`angularInset`  

A radius for the corners of the sector.

## Discussion

Use this initializer to map angular positions to a sector for each data element.

