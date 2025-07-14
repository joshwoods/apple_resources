

- Vision
- TargetedImageRequestHandler
-  init(sourceURL:targetURL:orientation:) 

Initializer

# init(sourceURL:targetURL:orientation:)

Creates a handler for performing requests on an image at the specified URL.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
convenience init(
    sourceURL: URL,
    targetURL: URL,
    orientation: CGImagePropertyOrientation? = nil
)
```

## See Also

### Creating a request handler

convenience init(source: Data, target: Data, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on an image contained in a data object.

convenience init(source: CGImage, target: CGImage, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on Core Graphics images.

convenience init(source: CVPixelBuffer, target: CVPixelBuffer, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on a Core Video pixel buffer.

convenience init(source: CMSampleBuffer, target: CMSampleBuffer, orientation: CGImagePropertyOrientation?)

Creates a request handler that performs requests on an image contained within a sample buffer.

convenience init(source: CIImage, target: CIImage, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on Core Image images.

