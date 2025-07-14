

- Core Image
- CIContext
-  createCGImage(\_:from:format:colorSpace:deferred:) 

Instance Method

# createCGImage(\_:from:format:colorSpace:deferred:)

Creates a Quartz 2D image from a region of a Core Image image object with deferred rendering.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func createCGImage(
    _ image: CIImage,
    from fromRect: CGRect,
    format: CIFormat,
    colorSpace: CGColorSpace?,
    deferred: Bool
) -> CGImage?
```

## Parameters 

`image`  

A Core Image image object.

`fromRect`  

The region of the image to render.

`format`  

The pixel format of the image.

`colorSpace`  

The color space for the output image. This color space must conform to either the CGColorSpaceModel.rgb or CGColorSpaceModel.monochrome model and be compatible with the specified pixel format.

`deferred`  

If `true`, Core Image delays rendering until the output Quartz 2D image is itself to be rendered. If `false`, Core Image renders to the output Quartz 2D image immediately.

## Return Value

A Quartz 2D image. You are responsible for releasing the returned image when you no longer need it.

## Discussion

Renders a region of an image into a temporary buffer using the context, and then creates and returns a Quartz 2D image with the results.

## See Also

### Rendering Images

func createCGImage(CIImage, from: CGRect) -> CGImage?

Creates a Quartz 2D image from a region of a Core Image image object.

func createCGImage(CIImage, from: CGRect, format: CIFormat, colorSpace: CGColorSpace?) -> CGImage?

Creates a Quartz 2D image from a region of a Core Image image object.

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

