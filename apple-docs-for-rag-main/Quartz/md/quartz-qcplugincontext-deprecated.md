

- Quartz
-  QCPlugInContext Deprecated

Protocol

# QCPlugInContext

The `QCPlugInContext` protocol defines methods that you use only from within the execution method (execute(_:atTime:withArguments:)) of a `QCPlugIn` object.

macOS 10.4–10.15Deprecated

``` source
protocol QCPlugInContext
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Topics

### Getting the OpenGL Context

func cglContextObj() -> CGLContextObj!

Returns the destination CGL context to use for OpenGL rendering from within the execution method.

**Required**

### Getting Execution Context Information

func userInfo() -> NSMutableDictionary!

Returns a mutable dictionary that contains information that can be shared between all instances of the `QCPlugIn` subclass, running in the same Quartz Composer context.

**Required**

func bounds() -> NSRect

Returns the bounds of the rendering context.

**Required**

func colorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space used by the rendering context.

**Required**

### Getting an Image Provider

func outputImageProviderFromBuffer(withPixelFormat: String!, pixelsWide: Int, pixelsHigh: Int, baseAddress: UnsafeRawPointer!, bytesPerRow: Int, releaseCallback: QCPlugInBufferReleaseCallback!, releaseContext: UnsafeMutableRawPointer!, colorSpace: CGColorSpace!, shouldColorMatch: Bool) -> Any!

Returns an image provider from a single memory buffer.

**Required**

func outputImageProviderFromTexture(withPixelFormat: String!, pixelsWide: Int, pixelsHigh: Int, name: GLuint, flipped: Bool, releaseCallback: QCPlugInTextureReleaseCallback!, releaseContext: UnsafeMutableRawPointer!, colorSpace: CGColorSpace!, shouldColorMatch: Bool) -> Any!

Returns an image provider from an OpenGL texture.

**Required**

### Instance Methods

func compositionURL() -> URL!

**Required**

## See Also

### Protocols

QCCompositionParameterViewDelegate

A protocol for composition parameter view’s delegate.

QCCompositionPickerViewDelegate

The `QCCompositionPickerViewDelegate` informal protocol defines methods that allow your application to respond to changes in a composition picker view (a QCCompositionPickerView object).

protocol QCCompositionRenderer

The `QCRenderer` protocol defines the methods used to pass data to the input ports or retrieve data from the output ports of the root patch of a Quartz Composer composition. This protocol is adopted by the QCRenderer, QCView, and QCCompositionLayer classes.

Deprecated

protocol QCPlugInInputImageSource

The `QCPlugInInputImageSource` protocol eliminates the need to use explicit image types for the image input ports on your custom patch. Not only does using the protocol avoid restrictions of a specific image type, but it avoids impedance mismatches, and provides better performance by deferring pixel computation until it is needed. When you need to access the pixels in an image, you simply convert the image to a representation (texture or buffer) using one of the methods defined by the `QCPlugInInputImageSource` protocol. Use a texture representation when you want to use input images on the GPU. Use a buffer representation when you want to use input images on the CPU.

Deprecated

protocol QCPlugInOutputImageProvider

The `QCPlugInOuputImageProvider` protocol eliminates the need to use explicit image types for the image output ports on a custom patch. The methods in this protocol are called by the Quartz Composer engine when the output image is needed. If your custom patch has an image output port, you need to implement the appropriate methods for rendering image data and to supply information about the rendering destination and the image bounds.

Deprecated

