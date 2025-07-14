

- VisionKit
- ImageAnalyzer
-  analyze(\_:configuration:) 

Instance Method

# analyze(\_:configuration:)

Returns the data for providing a Live Text interaction with an image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
final func analyze(
    _ image: UIImage,
    configuration: ImageAnalyzer.Configuration
) async throws -> ImageAnalysis
```

## Parameters 

`image`  

An image that the analyzer processes.

`configuration`  

A configuration that specifies the data types, and locales for text items, to recognize.

## Return Value

The data items that the analyzer finds in the image.

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

This function configures orientation automatically based on the given image’s orientation property.

## See Also

### Finding items in images

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

func analyze(imageAt: URL, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with an image at a URL and in the specified orientation.

