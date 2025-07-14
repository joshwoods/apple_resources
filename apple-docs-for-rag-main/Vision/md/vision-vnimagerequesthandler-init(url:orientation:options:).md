

- Vision
- VNImageRequestHandler
-  init(url:orientation:options:) 

Initializer

# init(url:orientation:options:)

Creates a handler to be used for performing requests on an image with known orientation, at the specified URL.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    url imageURL: URL,
    orientation: CGImagePropertyOrientation,
    options: [VNImageOption : Any] = [:]
)
```

## Parameters 

`imageURL`  

A URL pointing to the image to be used for performing the requests. The image must be in a format supported by Image I/O. Image content is immutable.

`orientation`  

The orientation of the input `image`.

`options`  

An optional dictionary containing VNImageOption keys to auxiliary image data.

## See Also

### Creating a Request Handler

init(cgImage: CGImage, options: [VNImageOption : Any])

Creates a handler to be used for performing requests on Core Graphics images.

init(cgImage: CGImage, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any])

Creates a handler to be used for performing requests on a Core Graphics image with known orientation.

init(ciImage: CIImage, options: [VNImageOption : Any])

Creates a handler to use for performing requests on Core Image image data.

init(ciImage: CIImage, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any])

Creates a handler to be used for performing requests on Core Image image data of a known orientation.

init(cvPixelBuffer: CVPixelBuffer, options: [VNImageOption : Any])

Creates a handler for performing requests on a Core Video pixel buffer.

init(cvPixelBuffer: CVPixelBuffer, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any])

Creates a handler for performing requests on a Core Video pixel buffer of a known orientation.

init(cvPixelBuffer: CVPixelBuffer, depthData: AVDepthData, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any])

init(cmSampleBuffer: CMSampleBuffer, options: [VNImageOption : Any])

Creates a request handler that performs requests on an image contained within a sample buffer.

init(cmSampleBuffer: CMSampleBuffer, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any])

Creates a request handler that performs requests on an image of a specified orientation contained within a sample buffer.

init(cmSampleBuffer: CMSampleBuffer, depthData: AVDepthData, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any])

Creates a request handler that performs requests on an image in a sample buffer that contains depth data.

init(data: Data, options: [VNImageOption : Any])

Creates a handler to use for performing requests on an image in a data object.

init(data: Data, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any])

Creates a handler to use for performing requests on an image of known orientation.

init(url: URL, options: [VNImageOption : Any])

Creates a handler to be used for performing requests on an image at the specified URL.

