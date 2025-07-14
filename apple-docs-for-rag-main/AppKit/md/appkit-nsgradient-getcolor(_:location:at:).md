

- AppKit
- NSGradient
-  getColor(\_:location:at:) 

Instance Method

# getColor(\_:location:at:)

Returns information about the color stop at the specified index in the receiver’s color array.

macOS 10.5+

``` source
func getColor(
    _ color: AutoreleasingUnsafeMutablePointer?,
    location: UnsafeMutablePointer?,
    at index: Int
)
```

## Parameters 

`color`  

On input, a pointer to a color object. On output, the color at the specified index in the receiver’s color array. You may specify `nil` if you are not interested in this parameter.

`location`  

On input, a pointer to a floating point number. On output, contains the location value associated with the color. This value is between 0.0 and 1.0. It is used to determine the position of the color relative to the start and end points of the gradient. You may specify `NULL` if you are not interested in this parameter.

`index`  

The index of the color you want.

## Discussion

This method returns the color stop information that was used to create the receiver. It does not return the interpolated color values at any point along the gradient. The location of the gradient’s first color is typically 0.0 and the location of the last color is typically 1.0, although the locations can vary depending on how the receiver was created.

## See Also

### Getting Gradient Properties

var colorSpace: NSColorSpace

The color space of the colors associated with the gradient.

var numberOfColorStops: Int

The number of color stops associated with the gradient.

func interpolatedColor(atLocation: CGFloat) -> NSColor

Returns the color of the rendered gradient at the specified relative location.

