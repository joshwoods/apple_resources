

- Vision
- VNTargetedImageRequest
-  init(targetedCMSampleBuffer:options:completionHandler:) 

Initializer

# init(targetedCMSampleBuffer:options:completionHandler:)

Creates a new request with a completion handler that targets an image in a sample buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(
    targetedCMSampleBuffer sampleBuffer: CMSampleBuffer,
    options: [VNImageOption : Any] = [:],
    completionHandler: VNRequestCompletionHandler? = nil
)
```

## Parameters 

`sampleBuffer`  

A sample buffer containing a valid imageBuffer.

`options`  

A dictionary with options specifying auxiliary information for the image.

`completionHandler`  

The callback the system invokes when the request finishes executing.

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

init(targetedCVPixelBuffer: CVPixelBuffer, orientation: CGImagePropertyOrientation, options: [VNImageOption : Any], completionHandler: VNRequestCompletionHandler?)

Creates a new request targeting an image in a pixel buffer of known orientation.

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

