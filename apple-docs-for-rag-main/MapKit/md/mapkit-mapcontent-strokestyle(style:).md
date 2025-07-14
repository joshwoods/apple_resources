

- MapKit
- MapContent
-  strokeStyle(style:) 

Instance Method

# strokeStyle(style:)

Applies the given stroke style to drawn map overlays.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
func strokeStyle(style: StrokeStyle) -> some MapContent
```

## Parameters 

`style`  

The stroke style to apply.

## Return Value

Returns MapContent with overlays drawn with the StrokeStyle you specified.

## See Also

### Setting stroke properties

func stroke(some ShapeStyle, lineWidth: CGFloat) -> some MapContent

Applies the given shape style to drawn map overlays using the line width you specify.

func stroke(some ShapeStyle, style: StrokeStyle) -> some MapContent

Applies the given shape style to drawn map overlays using the stroke style you specify.

func stroke(lineWidth: CGFloat) -> some MapContent

Applies the given stoke drawn map overlays using the line width you specify.

