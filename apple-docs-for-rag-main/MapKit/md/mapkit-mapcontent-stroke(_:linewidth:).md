

- MapKit
- MapContent
-  stroke(\_:lineWidth:) 

Instance Method

# stroke(\_:lineWidth:)

Applies the given shape style to drawn map overlays using the line width you specify.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
func stroke(
    _ content: some ShapeStyle,
    lineWidth: CGFloat = 1
) -> some MapContent
```

## Parameters 

`content`  

The shape style to apply.

`lineWidth`  

The line width to draw the stroke with.

## Return Value

Returns MapContent drawn with the ShapeStyle and `lineWidth` you specified.

## See Also

### Setting stroke properties

func stroke(some ShapeStyle, style: StrokeStyle) -> some MapContent

Applies the given shape style to drawn map overlays using the stroke style you specify.

func stroke(lineWidth: CGFloat) -> some MapContent

Applies the given stoke drawn map overlays using the line width you specify.

func strokeStyle(style: StrokeStyle) -> some MapContent

Applies the given stroke style to drawn map overlays.

