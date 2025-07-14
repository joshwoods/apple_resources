

- VisionKit
-  RecognizedItem 

Enumeration

# RecognizedItem

An item that the data scanner recognizes in the camera’s live video.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
enum RecognizedItem
```

## Mentioned in 

Scanning data with the camera

## Overview

A `RecognizedItem` enumeration contains the data for an item that the scanner identifies, such as the location, bounds, and content of the item. For text items, the content is the selected string, and for barcodes, it’s the encoded payload string.

## Topics

### Machine-readable items

case barcode(RecognizedItem.Barcode)

A machine-readable barcode.

struct Barcode

An object that represents a machine-readable code that the scanner recognizes.

### Text items

case text(RecognizedItem.Text)

Text or data the analyzer detects in text.

struct Text

An object that represents a text item that the scanner recognizes.

### Item location

var bounds: RecognizedItem.Bounds

The four corners of the recognized item in view coordinates.

struct Bounds

An object that represents the four corners of a recognized item.

### Item identification

var id: UUID

A unique identifier for the recognized item.

## Relationships

### Conforms To

- Identifiable

## See Also

### Barcode and text scanning through the camera

Scanning data with the camera

Enable Live Text data scanning of text and codes that appear in the camera’s viewfinder.

class DataScannerViewController

An object that scans the camera live video for text, data in text, and machine-readable codes.

protocol DataScannerViewControllerDelegate

A delegate object that responds when people interact with items that the data scanner recognizes.

