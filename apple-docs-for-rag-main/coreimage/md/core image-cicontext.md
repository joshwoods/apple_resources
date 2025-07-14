

- Core Image
-  CIContext 

Class

# CIContext

An evaluation context for rendering image processing results and performing image analysis.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class CIContext : NSObject
```

## Overview

The `CIContext` class provides an evaluation context for Core Image processing with Quartz 2D, Metal, or OpenGL. You use `CIContext` objects in conjunction with other Core Image classes, such as CIFilter, CIImage, and CIColor, to process images using Core Image filters. You also use a Core Image context with the CIDetector class to analyze images—for example, to detect faces or barcodes.

`CIContext` and CIImage objects are immutable, so multiple threads can use the same `CIContext` object to render `CIImage` objects. However, CIFilter objects are mutable and thus cannot be shared safely among threads. Each thread must create its own `CIFilter` objects, but you can pass a filter’s immutable input and output `CIImage` objects between threads.

## Topics

### Creating a Context Without Specifying a Destination

init()

Initializes a context without a specific rendering destination, using default options.

init(options: [CIContextOption : Any]?)

Initializes a context without a specific rendering destination, using the specified options.

### Creating a Context for CPU-Based Rendering

init(cgContext: CGContext, options: [CIContextOption : Any]?)

Creates a Core Image context from a Quartz context, using the specified options.

### Creating a Context for GPU-Based Rendering

init(mtlDevice: any MTLDevice)

Creates a Core Image context using the specified Metal device.

init(mtlDevice: any MTLDevice, options: [CIContextOption : Any]?)

Creates a Core Image context using the specified Metal device and options.

init(mtlCommandQueue: any MTLCommandQueue)

init(mtlCommandQueue: any MTLCommandQueue, options: [CIContextOption : Any]?)

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

func render(CIImage, to: CVPixelBuffer, bounds: CGRect, colorSpace: CGColorSpace?)

Renders a region of an image into a pixel buffer.

func render(CIImage, to: IOSurfaceRef, bounds: CGRect, colorSpace: CGColorSpace?)

Renders a region of an image into an IOSurface object.

func render(CIImage, to: any MTLTexture, commandBuffer: (any MTLCommandBuffer)?, bounds: CGRect, colorSpace: CGColorSpace)

Renders a region of an image to a Metal texture.

### Drawing Images

func draw(CIImage, at: CGPoint, from: CGRect)

Renders a region of an image to a point in the context destination.

func draw(CIImage, in: CGRect, from: CGRect)

Renders a region of an image to a rectangle in the context destination.

### Determining the Allowed Extents for Images Used by a Context

func inputImageMaximumSize() -> CGSize

Returns the maximum size allowed for any image rendered into the context.

func outputImageMaximumSize() -> CGSize

Returns the maximum size allowed for any image created by the context.

### Managing Resources

func clearCaches()

Frees any cached data, such as temporary images, associated with the context and runs the garbage collector.

func reclaimResources()

Runs the garbage collector to reclaim any resources that the context no longer requires.

class func offlineGPUCount() -> UInt32

Returns the number of GPUs not currently driving a display.

var workingColorSpace: CGColorSpace?

The working color space of the Core Image context.

var workingFormat: CIFormat

The working pixel format of the Core Image context.

### Rendering Images for Data or File Export

func tiffRepresentation(of: CIImage, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data?

Renders the image and exports the resulting image data in TIFF format.

func jpegRepresentation(of: CIImage, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data?

Renders the image and exports the resulting image data in JPEG format.

func pngRepresentation(of: CIImage, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data?

Renders the image and exports the resulting image data in PNG format.

func heifRepresentation(of: CIImage, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data?

Renders the image and exports the resulting image data in HEIF format.

func heif10Representation(of: CIImage, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data

Renders the image and exports the resulting image data in HEIF10 format.

func openEXRRepresentation(of: CIImage, options: [CIImageRepresentationOption : Any]) -> Data

Renders the image and exports the resulting image data in open EXR format.

func writeTIFFRepresentation(of: CIImage, to: URL, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in TIFF format.

func writeJPEGRepresentation(of: CIImage, to: URL, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in JPEG format.

func writePNGRepresentation(of: CIImage, to: URL, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in PNG format.

func writeHEIFRepresentation(of: CIImage, to: URL, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in HEIF format.

func writeHEIF10Representation(of: CIImage, to: URL, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in HEIF10 format.

func writeOpenEXRRepresentation(of: CIImage, to: URL, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in open EXR format.

struct CIImageRepresentationOption

### Creating Depth Blur Filters

func depthBlurEffectFilter(for: CIImage, disparityImage: CIImage, portraitEffectsMatte: CIImage?, hairSemanticSegmentation: CIImage?, glassesMatte: CIImage?, gainMap: CIImage?, orientation: CGImagePropertyOrientation, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(for: CIImage, disparityImage: CIImage, portraitEffectsMatte: CIImage?, hairSemanticSegmentation: CIImage?, orientation: CGImagePropertyOrientation, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(for: CIImage, disparityImage: CIImage, portraitEffectsMatte: CIImage?, orientation: CGImagePropertyOrientation, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(forImageData: Data, options: [AnyHashable : Any]?) -> CIFilter?

func depthBlurEffectFilter(forImageURL: URL, options: [AnyHashable : Any]?) -> CIFilter?

### Constants

Keys to be used in the `options` dictionary when creating a `CIContext` object.

struct CIContextOption

### Customizing Render Destination

func prepareRender(CIImage, from: CGRect, to: CIRenderDestination, at: CGPoint)

An optional call to warm up a CIContext so that subsequent calls to render with the same arguments run more efficiently.

func startTask(toClear: CIRenderDestination) -> CIRenderTask

Fills the entire destination with black or clear depending on its alphaMode.

func startTask(toRender: CIImage, from: CGRect, to: CIRenderDestination, at: CGPoint) -> CIRenderTask

Renders a portion of an image to a point in the destination.

func startTask(toRender: CIImage, to: CIRenderDestination) -> CIRenderTask

Renders an image to a destination so that point (0, 0) of the image maps to point (0, 0) of the destination.

### Deprecated

init(cglContext: CGLContextObj, pixelFormat: CGLPixelFormatObj?, colorSpace: CGColorSpace?, options: [CIContextOption : Any]?)

Creates a Core Image context from a CGL context, using the specified options, color space, and pixel format object.

Deprecated

init(eaglContext: EAGLContext)

Creates a Core Image context from an EAGL context.

Deprecated

init(eaglContext: EAGLContext, options: [CIContextOption : Any]?)

Creates a Core Image context from an EAGL context using the specified options.

Deprecated

init?(forOfflineGPUAt: UInt32)

Creates an OpenGL-based Core Image context using a GPU that is not currently driving a display.

Deprecated

init?(forOfflineGPUAt: UInt32, colorSpace: CGColorSpace?, options: [CIContextOption : Any]?, sharedContext: CGLContextObj?)

Creates an OpenGL-based Core Image context using a GPU that is not currently driving a display, with the specified options.

Deprecated

func createCGLayer(with: CGSize, info: CFDictionary?) -> CGLayer?

Creates a CGLayer object from the provided parameters.

Deprecated

## Relationships

### Inherits From

- NSObject

## See Also

### Essentials

Processing an Image Using Built-in Filters

Apply effects such as sepia tint, highlight strengthening, and scaling to images.

class CIImage

A representation of an image to be processed or produced by Core Image filters.

