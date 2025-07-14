

- VisionKit
- ImageAnalyzer
-  analyze(imageAt:orientation:configuration:) 

Instance Method

# analyze(imageAt:orientation:configuration:)

Returns the data for providing a Live Text interaction with an image at a URL and in the specified orientation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
final func analyze(
    imageAt url: URL,
    orientation: CGImagePropertyOrientation,
    configuration: ImageAnalyzer.Configuration
) async throws -> ImageAnalysis
```

## Parameters 

`url`  

The URL location of an image that the analyzer processes.

`orientation`  

The orientation that the analyzer uses to process the image.

`configuration`  

A configuration that specifies the data types, and locales for text items, to recognize.

## Return Value

The data items that the analyzer finds in the image.

## See Also

### Finding items in images

func analyze(UIImage, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with an image.

func analyze(NSImage, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with an image in the specified orientation.

func analyze(CGImage, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with a Core Graphics image in the specified orientation.

func analyze(CVPixelBuffer, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with a pixel buffer image in the specified orientation.

func analyze(CIImage, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with a bitmap image in the specified orientation.

func analyze(UIImage, orientation: UIImage.Orientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with an image in the specified orientation.

