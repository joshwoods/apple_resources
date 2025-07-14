

- Image I/O
-  kCGImagePropertyHasAlpha 

Global Variable

# kCGImagePropertyHasAlpha

A Boolean value that indicates whether the image has an alpha channel.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImagePropertyHasAlpha: CFString
```

## Discussion

The value of this key is a CFBoolean. The value is kCFBooleanTrue when the image contains an alpha channel.

## See Also

### Color Information

let kCGImagePropertyNamedColorSpace: CFString

The name of the image’s color space.

let kCGImagePropertyProfileName: CFString

The name of the optional International Color Consortium (ICC) profile embedded in the image, if known.

let kCGImagePropertyColorModel: CFString

The color model of the image, such as RGB, CMYK, grayscale, or Lab.

let kCGImagePropertyColorModelRGB: CFString

A Red Green Blue (RGB) color model.

let kCGImagePropertyColorModelCMYK: CFString

A Cyan Magenta Yellow Black (CMYK) color model.

let kCGImagePropertyColorModelGray: CFString

A grayscale color model.

let kCGImagePropertyColorModelLab: CFString

A Lab color model, where color values contain the amount of light and the amounts of four human-perceivable colors.

