

- Vision
- ImageProcessingRequest
-  perform(on:orientation:) 

Instance Method

# perform(on:orientation:)

Performs the request on a Core Media buffer and produces observations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func perform(
    on sampleBuffer: CMSampleBuffer,
    orientation: CGImagePropertyOrientation?
) async throws -> Self.Result
```

**Required** Default implementations provided.

## Parameters 

`sampleBuffer`  

The input CMSampleBuffer on which to perform the request.

`orientation`  

The orientation of the input image. Default is `nil`.

## Return Value

The observation — or list of observations — the request produces.

## Default Implementations

### ImageProcessingRequest Implementations

func perform(on: CVPixelBuffer, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

func perform(on: CIImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

func perform(on: CMSampleBuffer, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

func perform(on: CGImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

func perform(on: Data, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

func perform(on: URL, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

## See Also

### Performing a request

func perform(on: URL, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on an image URL and produces observations.

**Required** Default implementations provided.

func perform(on: Data, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on image data and produces observations.

**Required** Default implementations provided.

func perform(on: CGImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Graphics image and produces observations.

**Required** Default implementations provided.

func perform(on: CVPixelBuffer, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a pixel buffer and produces observations.

**Required** Default implementations provided.

func perform(on: CIImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Image image and produces observations.

**Required** Default implementations provided.

struct ImageAestheticsScoresObservation

An observation that provides an overall score of aesthetic attributes for an image.

