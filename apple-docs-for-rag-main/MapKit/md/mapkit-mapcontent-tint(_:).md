

- MapKit
- MapContent
-  tint(\_:) 

Instance Method

# tint(\_:)

The tint shape style to apply to map content.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
func tint(_ tint: S) -> some MapContent where S : ShapeStyle
```

## Parameters 

`tint`  

The tint to apply.

## Return Value

Returns MapContent with overlays drawn with the ShapeStyle you specified.

## See Also

### Setting the content style

func foregroundStyle(some ShapeStyle) -> some MapContent

Specifies the shape style used to fill content in drawing map overlays.

