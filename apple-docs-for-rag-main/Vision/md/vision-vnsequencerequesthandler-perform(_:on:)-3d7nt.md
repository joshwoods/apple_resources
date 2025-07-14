

- Vision
- VNSequenceRequestHandler
-  perform(\_:on:) 

Instance Method

# perform(\_:on:)

Schedules one or more Vision requests to be performed on a Core Video pixel buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func perform(
    _ requests: [VNRequest],
    on pixelBuffer: CVPixelBuffer
) throws
```

## Parameters 

`requests`  

An array of VNRequest requests to perform.

`pixelBuffer`  

The input CVPixelBuffer on which to perform the request.

## See Also

### Performing a Sequence Request

func perform([VNRequest], on: CGImage) throws

Schedules Vision requests to be performed on a Core Graphics image.

func perform([VNRequest], on: CGImage, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on a Core Graphics image with known orientation.

func perform([VNRequest], on: CIImage) throws

Schedules one or more Vision requests to be performed on Core Image image data.

func perform([VNRequest], on: CIImage, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on Core Image image data with known orientation.

func perform([VNRequest], on: CVPixelBuffer, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on a Core Video pixel buffer with known orientation.

func perform([VNRequest], on: CMSampleBuffer) throws

Performs one or more requests on an image contained within a sample buffer.

func perform([VNRequest], on: CMSampleBuffer, orientation: CGImagePropertyOrientation) throws

Performs one or more requests on an image of a specified orientation contained within a sample buffer.

func perform([VNRequest], onImageData: Data) throws

Schedules one or more Vision requests to be performed on raw image data.

func perform([VNRequest], onImageData: Data, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on raw data containing an image with known orientation.

func perform([VNRequest], onImageURL: URL) throws

Schedules one or more Vision requests to be performed on an image.

func perform([VNRequest], onImageURL: URL, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on an image with known orientation, at a specific URL.

