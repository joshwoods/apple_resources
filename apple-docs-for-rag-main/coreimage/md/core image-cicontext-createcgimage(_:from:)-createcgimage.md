

- Core Image
- CIContext
-  createCGImage(\_:from:) 

Instance Method

# createCGImage(\_:from:)

Creates a Quartz 2D image from a region of a Core Image image object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func createCGImage(
    _ image: CIImage,
    from fromRect: CGRect
) -> CGImage?
```

## Parameters 

`im`  

A Core Image image object.

`r`  

The region of the image to render.

## Return Value

A Quartz 2D image. You are responsible for releasing the returned image when you no longer need it.

## Discussion

Renders a region of an image into a temporary buffer using the context, then creates and returns a Quartz 2D image with the results.

## See Also

### Rendering Images

func createCGImage(CIImage, from: CGRect, format: CIFormat, colorSpace: CGColorSpace?) -> CGImage?

Creates a Quartz 2D image from a region of a Core Image image object.

func createCGImage(CIImage, from: CGRect, format: CIFormat, colorSpace: CGColorSpace?, deferred: Bool) -> CGImage?

Creates a Quartz 2D image from a region of a Core Image image object with deferred rendering.

func render(CIImage, toBitmap: UnsafeMutableRawPointer, rowBytes: Int, bounds: CGRect, format: CIFormat, colorSpace: CGColorSpace?)

Renders to the given bitmap.

func render(CIImage, to: CVPixelBuffer)

Renders an image into a pixel buffer.

func render(CIImage, to: CVPixelBuffer, bounds: CGRect, colorSpace: CGColorSpace?)

Renders a region of an image into a pixel buffer.

func render(CIImage, to: IOSurfaceRef, bounds: CGRect, colorSpace: CGColorSpace?)

Renders a region of an image into an IOSurface object.

func render(CIImage, to: any MTLTexture, commandBuffer: (any MTLCommandBuffer)?, bounds: CGRect, colorSpace: CGColorSpace)

Renders a region of an image to a Metal texture.

