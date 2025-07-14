

- Image I/O
-  kCGImagePropertyProfileName 

Global Variable

# kCGImagePropertyProfileName

The name of the optional International Color Consortium (ICC) profile embedded in the image, if known.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImagePropertyProfileName: CFString
```

## Discussion

The value of this key is a CFString.

## See Also

### Color Information

let kCGImagePropertyHasAlpha: CFString

A Boolean value that indicates whether the image has an alpha channel.

let kCGImagePropertyNamedColorSpace: CFString

The name of the image’s color space.

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

