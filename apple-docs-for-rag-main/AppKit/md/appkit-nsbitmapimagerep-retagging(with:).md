

- AppKit
- NSBitmapImageRep
-  retagging(with:) 

Instance Method

# retagging(with:)

Changes the color space tag of the bitmap image representation.

macOS 10.6+

``` source
func retagging(with newSpace: NSColorSpace) -> NSBitmapImageRep?
```

## Parameters 

`newSpace`  

The desired color space.

## Return Value

An NSBitmapImageRep, or `nil`, if the conversion fails. If the original NSBitmapImageRep already uses that color space, it is returned as is.

## Discussion

This method will definitely fail if you pass a color space that has a different color space model than the receiver. That is, if your original image is sRGB, you can only retag with some other RGB colorspace.

## See Also

### Managing Color Spaces

func converting(to: NSColorSpace, renderingIntent: NSColorRenderingIntent) -> NSBitmapImageRep?

Converts the bitmap image representation to the specified color space.

var colorSpace: NSColorSpace

The color space of the bitmap.

