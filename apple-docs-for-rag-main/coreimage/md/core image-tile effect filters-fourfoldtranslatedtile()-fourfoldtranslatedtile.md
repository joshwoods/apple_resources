

- Core Image
- Tile Effect Filters
-  fourfoldTranslatedTile() 

Type Method

# fourfoldTranslatedTile()

Creates a tiled image by applying four translation operations.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func fourfoldTranslatedTile() -> any CIFilter & CIFourfoldTranslatedTile
```

## Return Value

The tiled image.

## Discussion

This method applies the four-fold translated tile filter to an image. The effect produces a four-way tiled image by applying four translation operations. Translation operations map the position of each element in the photo to a new position in the output image.

The four-fold translated tile filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`center`  
A set of coordinates marking the center of the image as a CGPoint. This controls the source of the tile contents.

`angle`  
A `float` representing the direction of the tiled patten, in radians as an NSNumber.

`width`  
A `float` representing the set width of each tile as an `NSNumber`.

`acuteAngle`  
A `float` representing the primary angle for the repeating translated tile as an `NSNumber`.

The following code creates a filter that performs a four-fold translated tile operation on the image:

func fourFoldTranslated(inputImage: CIImage) -> CIImage {
    let fourFoldTranslatedTile = CIFilter.fourfoldTranslatedTile()
    fourFoldTranslatedTile.inputImage = inputImage
    fourFoldTranslatedTile.center = CGPoint(x: inputImage.extent.midX, y: inputImage.extent.midY)
    fourFoldTranslatedTile.angle = 1
    fourFoldTranslatedTile.width = 400
    fourFoldTranslatedTile.acuteAngle = 1
    return fourFoldTranslatedTile.outputImage!.cropped(to: inputImage.extent)
}

## See Also

### Filters

class func affineClamp() -> any CIFilter &amp; CIAffineClamp

Performs a transform on the image and extends the image edges to infinity.

class func affineTile() -> any CIFilter &amp; CIAffineTile

Performs a transform on the image and tiles the result.

class func eightfoldReflectedTile() -> any CIFilter &amp; CIEightfoldReflectedTile

Creates an eight-way reflected pattern.

class func fourfoldReflectedTile() -> any CIFilter &amp; CIFourfoldReflectedTile

Creates a four-way reflected pattern.

class func fourfoldRotatedTile() -> any CIFilter &amp; CIFourfoldRotatedTile

Creates a tiled image by rotating a tile in increments of 90 degrees.

class func glideReflectedTile() -> any CIFilter &amp; CIGlideReflectedTile

Tiles an image by rotating and reflecting a tile from the image.

class func kaleidoscope() -> any CIFilter &amp; CIKaleidoscope

Creates a 12-way kaleidoscopic image from an image.

class func opTile() -> any CIFilter &amp; CIOpTile

Produces an effect that mimics a style of visual art that uses optical illusions.

class func parallelogramTile() -> any CIFilter &amp; CIParallelogramTile

Warps the image to create a parallelogram and tiles the result.

class func perspectiveTile() -> any CIFilter &amp; CIPerspectiveTile

Tiles an image by adjusting the perspective of the image.

class func sixfoldReflectedTile() -> any CIFilter &amp; CISixfoldReflectedTile

Produces a tiled image from a source image by applying a six-way reflected symmetry.

class func sixfoldRotatedTile() -> any CIFilter &amp; CISixfoldRotatedTile

Creates a tiled image by rotating in increments of 60 degrees.

class func triangleKaleidoscope() -> any CIFilter &amp; CITriangleKaleidoscope

Create a triangular kaleidoscope effect and then tiles the result.

class func triangleTile() -> any CIFilter &amp; CITriangleTile

Tiles a triangular area of an image.

class func twelvefoldReflectedTile() -> any CIFilter &amp; CITwelvefoldReflectedTile

Creates a tiled image by rotating in increments of 30 degrees.

