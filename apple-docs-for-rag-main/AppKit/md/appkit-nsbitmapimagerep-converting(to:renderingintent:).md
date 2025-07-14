

- AppKit
- NSBitmapImageRep
-  converting(to:renderingIntent:) 

Instance Method

# converting(to:renderingIntent:)

Converts the bitmap image representation to the specified color space.

macOS 10.6+

``` source
func converting(
    to targetSpace: NSColorSpace,
    renderingIntent: NSColorRenderingIntent
) -> NSBitmapImageRep?
```

## Parameters 

`targetSpace`  

The new color space.

`renderingIntent`  

The rendering intent specifies how to handle colors that are not located within the target color space. The supported values are NSColorRenderingIntent.

## Return Value

An NSBitmapImageRep, or `nil`, if the conversion fails. If the original NSBitmapImageRep already uses that color space, it is returned as is.

## See Also

### Managing Color Spaces

func retagging(with: NSColorSpace) -> NSBitmapImageRep?

Changes the color space tag of the bitmap image representation.

var colorSpace: NSColorSpace

The color space of the bitmap.

