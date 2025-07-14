

- Vision
- VNTargetedImageRequest
-  init(targetedCVPixelBuffer:orientation:options:completionHandler:) 

Initializer

# init(targetedCVPixelBuffer:orientation:options:completionHandler:)

Creates a new request targeting an image in a pixel buffer of known orientation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    targetedCVPixelBuffer pixelBuffer: CVPixelBuffer,
    orientation: CGImagePropertyOrientation,
    options: [VNImageOption : Any] = [:],
    completionHandler: VNRequestCompletionHandler? = nil
)
```

## Parameters 

`pixelBuffer`  

The pixel buffer containing the targeted image.

`orientation`  

The orientation of the image buffer, based on EXIF specification and superseding other orientation information. The value must be an integer from `1` to `8`; see kCGImagePropertyOrientation for details.

`options`  

A dictionary with options specifying auxiliary information for the image.

`completionHandler`  

The block to invoke when the request has finished executing.

## See Also

### Creating a Request

init(targetedCGImage: CGImage, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting a Core Graphics image, executing the completion handler when done.

init(targetedCGImage: CGImage, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting a Core Graphics image of known orientation, executing the completion handler when done.

init(targetedCIImage: CIImage, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting a Core Image image.

init(targetedCIImage: CIImage, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting a Core Image image of known orientation, executing the completion handler when done.

init(targetedCVPixelBuffer: CVPixelBuffer, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting an image in a pixel buffer.

init(targetedCMSampleBuffer: CMSampleBuffer, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request with a completion handler that targets an image in a sample buffer.

init(targetedCMSampleBuffer: CMSampleBuffer, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request with a completion handler that targets an image of a known orientation in a sample buffer.

init(targetedImageData: Data, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting an image as raw data, executing the completion handler when done.

init(targetedImageData: Data, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting a raw data image of known orientation, executing the completion handler when done.

init(targetedImageURL: URL, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting an image at the specified URL, executing the completion handler when done.

init(targetedImageURL: URL, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting an image of known orientation, at the specified URL, executing the completion handler when done.

