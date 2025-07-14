

- MapKit
- MapContent
-  stroke(lineWidth:) 

Instance Method

# stroke(lineWidth:)

Applies the given stoke drawn map overlays using the line width you specify.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
func stroke(lineWidth: CGFloat = 1) -> some MapContent
```

## Parameters 

`lineWidth`  

The line width to draw the stroke with.

## Return Value

Returns MapContent with overlays drawn with `lineWidth` you specified.

## See Also

### Setting stroke properties

func stroke(some ShapeStyle, lineWidth: CGFloat) -> some MapContent

Applies the given shape style to drawn map overlays using the line width you specify.

func stroke(some ShapeStyle, style: StrokeStyle) -> some MapContent

Applies the given shape style to drawn map overlays using the stroke style you specify.

func strokeStyle(style: StrokeStyle) -> some MapContent

Applies the given stroke style to drawn map overlays.

