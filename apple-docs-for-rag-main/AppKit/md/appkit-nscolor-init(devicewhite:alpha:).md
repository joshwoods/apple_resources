

- AppKit
- NSColor
-  init(deviceWhite:alpha:) 

Initializer

# init(deviceWhite:alpha:)

Creates a color object using the given opacity and grayscale values.

macOS

``` source
init(
    deviceWhite white: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`white`  

The grayscale value of the color object.

`alpha`  

The opacity value of the color object.

## Return Value

The color object.

## Discussion

Values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

## See Also

### Related Documentation

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the grayscale and alpha values of the color.

### Creating a Color Using White Components

init(white: CGFloat, alpha: CGFloat)

Creates a color object with the specified brightness and alpha channel values.

init(calibratedWhite: CGFloat, alpha: CGFloat)

Creates a color object using the given opacity and grayscale values.

init(genericGamma22White: CGFloat, alpha: CGFloat)

Returns a color object with the specified white and alpha values in the GenericGamma22 colorspace.

