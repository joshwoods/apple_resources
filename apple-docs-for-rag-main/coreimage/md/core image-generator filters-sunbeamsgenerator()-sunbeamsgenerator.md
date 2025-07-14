

- Core Image
- Generator Filters
-  sunbeamsGenerator() 

Type Method

# sunbeamsGenerator()

Generates an image resembling the sun.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func sunbeamsGenerator() -> any CIFilter & CISunbeamsGenerator
```

## Return Value

The generated image.

## Discussion

This method generates a sunbeam as an image. The effect generates a center-textured sun with striations. You can combine with other filters to create more sophisticated images.

The sunbeams generator filter uses the following properties:

`center`  
A vector representing the center of the image as a CIVector.

`color`  
A CIColor representing the color of the sun.

`sunRadius`  
A `float` representing the radius of the center sun as an NSNumber.

`maxStriationRadius`  
A `float` representing the striation radius as an `NSNumber`.

`striationStrength`  
A `float` representing the striation strength as an `NSNumber`.

`striationContrast`  
A `float` representing the striation contrast as an `NSNumber`.

`time`  
A `float` representing the time as an `NSNumber`.

The following code creates a filter that generates an image that resembles a yellow sun with sunbeams:

    func sunBeam () -> CIImage {
        let sunBeamGenerator = CIFilter.sunbeamsGenerator()
        sunBeamGenerator.center = CGPoint(x: 150, y: 150)
        sunBeamGenerator.color = CIColor(red: 0.96, green: 1, blue: 1, alpha: 1)
        sunBeamGenerator.sunRadius = 40
        sunBeamGenerator.maxStriationRadius = 2.58
        sunBeamGenerator.striationStrength = 0.50
        sunBeamGenerator.striationContrast = 1.38
        sunBeamGenerator.time = 0
        return sunBeamGenerator.outputImage!
    }

## See Also

### Filters

class func attributedTextImageGenerator() -> any CIFilter &amp; CIAttributedTextImageGenerator

Generates an attributed-text image.

class func aztecCodeGenerator() -> any CIFilter &amp; CIAztecCodeGenerator

Generates a low-density barcode.

class func barcodeGenerator() -> any CIFilter &amp; CIBarcodeGenerator

Generates a barcode as an image from the descriptor.

class func blurredRectangleGenerator() -> any CIFilter &amp; CIBlurredRectangleGenerator

Generates a blurred rectangle.

class func checkerboardGenerator() -> any CIFilter &amp; CICheckerboardGenerator

Generates a checkerboard image.

class func code128BarcodeGenerator() -> any CIFilter &amp; CICode128BarcodeGenerator

Generates a high-density, linear barcode.

class func lenticularHaloGenerator() -> any CIFilter &amp; CILenticularHaloGenerator

Generates a lenticular halo image.

class func meshGenerator() -> any CIFilter &amp; CIMeshGenerator

Generates a pattern made from an array of line segments.

class func pdf417BarcodeGenerator() -> any CIFilter &amp; CIPDF417BarcodeGenerator

Generates a high-density linear barcode.

class func qrCodeGenerator() -> any CIFilter &amp; CIQRCodeGenerator

Generates a quick response (QR) code image.

class func randomGenerator() -> any CIFilter &amp; CIRandomGenerator

Generates a random filter image.

class func roundedRectangleGenerator() -> any CIFilter &amp; CIRoundedRectangleGenerator

Generates a rounded rectangle image.

class func roundedRectangleStrokeGenerator() -> any CIFilter &amp; CIRoundedRectangleStrokeGenerator

Creates an image containing the outline of a rounded rectangle.

class func starShineGenerator() -> any CIFilter &amp; CIStarShineGenerator

Generates a star-shine image.

class func stripesGenerator() -> any CIFilter &amp; CIStripesGenerator

Generates a line of stripes as an image

class func textImageGenerator() -> any CIFilter &amp; CITextImageGenerator

Generates a text image.

