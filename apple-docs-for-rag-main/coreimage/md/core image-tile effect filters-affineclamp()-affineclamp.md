

- Core Image
- Tile Effect Filters
-  affineClamp() 

Type Method

# affineClamp()

Performs a transform on the image and extends the image edges to infinity.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func affineClamp() -> any CIFilter & CIAffineClamp
```

## Return Value

The tiled image.

## Discussion

This method applies the affine clamp filter to an image. This effect performs similarly to the affine transform filter except that it produces an infinite image. You can use this filter when you need to blur an image but you want to avoid a soft, black fringe along the edges.

The affine clamp filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`transform`  
A CGAffineTransform to constrain to the image.

The following code creates a filter that produces a cropped image with colored edges to fill the rest of the image:

func affineClamp(inputImage: CIImage) -> CIImage {
    let affineClamp = CIFilter.affineClamp()
    affineClamp.inputImage = inputImage
    affineClamp.transform = CGAffineTransform(a: 1.0, b: 0.0, c: 0.0, d: 1.0, tx: 0.0, ty: 0.0)
    return affineClamp.outputImage!
}

## See Also

### Filters

class func affineTile() -> any CIFilter &amp; CIAffineTile

Performs a transform on the image and tiles the result.

class func eightfoldReflectedTile() -> any CIFilter &amp; CIEightfoldReflectedTile

Creates an eight-way reflected pattern.

class func fourfoldReflectedTile() -> any CIFilter &amp; CIFourfoldReflectedTile

Creates a four-way reflected pattern.

class func fourfoldRotatedTile() -> any CIFilter &amp; CIFourfoldRotatedTile

Creates a tiled image by rotating a tile in increments of 90 degrees.

class func fourfoldTranslatedTile() -> any CIFilter &amp; CIFourfoldTranslatedTile

Creates a tiled image by applying four translation operations.

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

