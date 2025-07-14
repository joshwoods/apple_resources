

- VisionKit
- ImageAnalyzer
-  ImageAnalyzer.AnalysisTypes 

Structure

# ImageAnalyzer.AnalysisTypes

The types of items that an image analyzer looks for in an image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
struct AnalysisTypes
```

## Topics

### Specifying types to find

static let machineReadableCode: ImageAnalyzer.AnalysisTypes

An option that analyzes an image for machine-readable codes, such as QR codes.

static let text: ImageAnalyzer.AnalysisTypes

An option that analyzes an image for text.

static let visualLookUp: ImageAnalyzer.AnalysisTypes

An option that analyzes an image for subjects that the framework can look up for more information.

### Managing sets

Set properties and methods

The properties and methods that conform to the option set protocol.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating configurations

init(ImageAnalyzer.AnalysisTypes)

Creates a configuration that an image analyzer uses to find items.

let analysisTypes: ImageAnalyzer.AnalysisTypes

The types of items that the image analyzer looks for in the image.

