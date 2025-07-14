

- Core Image
- Tile Effect Filters
-  perspectiveTile() 

Type Method

# perspectiveTile()

Tiles an image by adjusting the perspective of the image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func perspectiveTile() -> any CIFilter & CIPerspectiveTile
```

## Return Value

The tiled image.

## Discussion

This method applies the perspective tile filter to an image. The effect adjusts the perspective of the image and then tiles the result.

The perspective tile filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`topLeft`  
A CGPoint of the input image mapped to the top-left corner of the tile.

`topRight`  
A `CGPoint` of the input image mapped to the top-right corner of the tile.

`bottomLeft`  
A CGPoint of the input image mapped to the bottom-left corner of the tile.

`bottomRight`  
A `CGPoint` of the input image mapped to the bottom-right corner of the tile.

The following code creates a filter that tiles the image and adjusts the perspective to add depth:

func perspective(inputImage: CIImage) -> CIImage {
    let perspectiveTile = CIFilter.perspectiveTile()
    perspectiveTile.inputImage = inputImage
    perspectiveTile.topLeft = CGPoint(x: 118, y: 484)
    perspectiveTile.topRight = CGPoint(x: 646, y: 507)
    perspectiveTile.bottomLeft = CGPoint(x: 548, y: 140)
    perspectiveTile.bottomRight = CGPoint(x: 155, y: 153)
    return perspectiveTile.outputImage!
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

