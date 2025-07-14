

- Core Image
- CIFilter
-  Generator Filters 

API Collection

# Generator Filters

## Topics

### Filters

class func pdf417BarcodeGenerator() -> any CIFilter &amp; CIPDF417BarcodeGenerator

Generates a high-density linear barcode.

class func qrCodeGenerator() -> any CIFilter &amp; CIQRCodeGenerator

Generates a quick response (QR) code image.

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

class func sunbeamsGenerator() -> any CIFilter &amp; CISunbeamsGenerator

Generates an image resembling the sun.

class func textImageGenerator() -> any CIFilter &amp; CITextImageGenerator

Generates a text image.

### Protocols

protocol CICode128BarcodeGenerator

The properties you use to configure a Code 128 barcode generator filter.

protocol CIAttributedTextImageGenerator

The properties you use to configure an attributed-text image generator filter.

protocol CIAztecCodeGenerator

The properties you use to configure an Aztec code generator filter.

protocol CIBarcodeGenerator

The properties you use to configure a barcode generator filter.

protocol CIBlurredRectangleGenerator

protocol CICheckerboardGenerator

The properties you use to configure a checkerboard generator filter.

protocol CILenticularHaloGenerator

The properties you use to configure a lenticular halo generator filter.

protocol CIMeshGenerator

The properties you use to configure a mesh generator filter.

protocol CIPDF417BarcodeGenerator

The properties you use to configure a PDF417 barcode generator filter.

protocol CIQRCodeGenerator

The properties you use to configure a QR code generator filter.

protocol CIRandomGenerator

The properties you use to configure a random generator filter.

protocol CIRoundedRectangleGenerator

protocol CIRoundedRectangleStrokeGenerator

protocol CIStarShineGenerator

The properties you use to configure a star-shine generator filter.

protocol CIStripesGenerator

The properties you use to configure a stripes generator filter.

protocol CISunbeamsGenerator

The properties you use to configure a sunbeams generator filter.

protocol CITextImageGenerator

The properties you use to configure a text image generator filter.

## See Also

### Configuring Type-Safe Filters

protocol CIFilterProtocol

The properties you use to configure a Core Image filter.

Blur Filters

Color Adjustment Filters

Color Effect Filters

Composite Operations

Convolution Filters

Distortion Filters

Geometry Adjustment Filters

Gradient Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

