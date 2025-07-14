

- Vision
- ImageRequestHandler
-  init(\_:orientation:) 

Initializer

# init(\_:orientation:)

Creates a handler for performing requests on Core Image images.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
convenience init(
    _ image: CIImage,
    orientation: CGImagePropertyOrientation? = nil
)
```

## See Also

### Creating a request handler

convenience init(URL, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on an image at the specified URL.

convenience init(Data, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on an image contained in a data object.

convenience init(CGImage, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on Core Graphics images.

convenience init(CVPixelBuffer, depthData: AVDepthData?, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on a Core Video pixel buffer.

convenience init(CMSampleBuffer, depthData: AVDepthData?, orientation: CGImagePropertyOrientation?)

Creates a request handler that performs requests on an image contained within a sample buffer.

