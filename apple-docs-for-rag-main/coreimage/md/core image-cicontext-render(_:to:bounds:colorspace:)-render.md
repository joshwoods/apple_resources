

- Core Image
- CIContext
-  render(\_:to:bounds:colorSpace:) 

Instance Method

# render(\_:to:bounds:colorSpace:)

Renders a region of an image into a pixel buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func render(
    _ image: CIImage,
    to buffer: CVPixelBuffer,
    bounds: CGRect,
    colorSpace: CGColorSpace?
)
```

## Parameters 

`image`  

A Core Image image object.

`buffer`  

The destination pixel buffer.

`r`  

The rectangle in the destination pixel buffer to draw into.

`cs`  

The color space of the destination pixel buffer.

## See Also

### Rendering Images

func createCGImage(CIImage, from: CGRect) -> CGImage?

Creates a Quartz 2D image from a region of a Core Image image object.

func createCGImage(CIImage, from: CGRect, format: CIFormat, colorSpace: CGColorSpace?) -> CGImage?

Creates a Quartz 2D image from a region of a Core Image image object.

func createCGImage(CIImage, from: CGRect, format: CIFormat, colorSpace: CGColorSpace?, deferred: Bool) -> CGImage?

Creates a Quartz 2D image from a region of a Core Image image object with deferred rendering.

func render(CIImage, toBitmap: UnsafeMutableRawPointer, rowBytes: Int, bounds: CGRect, format: CIFormat, colorSpace: CGColorSpace?)

Renders to the given bitmap.

func render(CIImage, to: CVPixelBuffer)

Renders an image into a pixel buffer.

func render(CIImage, to: IOSurfaceRef, bounds: CGRect, colorSpace: CGColorSpace?)

Renders a region of an image into an IOSurface object.

func render(CIImage, to: any MTLTexture, commandBuffer: (any MTLCommandBuffer)?, bounds: CGRect, colorSpace: CGColorSpace)

Renders a region of an image to a Metal texture.

