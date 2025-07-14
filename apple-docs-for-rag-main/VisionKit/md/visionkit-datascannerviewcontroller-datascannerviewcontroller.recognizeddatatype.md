

- VisionKit
- DataScannerViewController
-  DataScannerViewController.RecognizedDataType 

Structure

# DataScannerViewController.RecognizedDataType

A type of data that the scanner recognizes.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
struct RecognizedDataType
```

## Mentioned in 

Scanning data with the camera

## Topics

### Recognizing text

static func text(languages: [String], textContentType: DataScannerViewController.TextContentType?) -> DataScannerViewController.RecognizedDataType

Creates a data type for text and information the scanner finds in text.

enum TextContentType

Types of text that a data scanner recognizes.

### Recognizing machine-readable codes

static func barcode(symbologies: [VNBarcodeSymbology]) -> DataScannerViewController.RecognizedDataType

Creates a data type for barcodes the use the specified symbologies.

### Hashing and comparing

func hash(into: inout Hasher)

Hashes the components of this value using the specified hasher.

static func == (DataScannerViewController.RecognizedDataType, DataScannerViewController.RecognizedDataType) -> Bool

Returns a Boolean value indicating whether two sets have equal elements.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Creating data scanners

init(recognizedDataTypes: Set&lt;DataScannerViewController.RecognizedDataType>, qualityLevel: DataScannerViewController.QualityLevel, recognizesMultipleItems: Bool, isHighFrameRateTrackingEnabled: Bool, isPinchToZoomEnabled: Bool, isGuidanceEnabled: Bool, isHighlightingEnabled: Bool)

Creates a scanner for finding data, such as text and machine-readable codes, in the camera’s live video.

let recognizedDataTypes: Set&lt;DataScannerViewController.RecognizedDataType>

The types of data that the data scanner identifies in the live video.

