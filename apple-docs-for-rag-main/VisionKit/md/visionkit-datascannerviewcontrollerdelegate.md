

- VisionKit
-  DataScannerViewControllerDelegate 

Protocol

# DataScannerViewControllerDelegate

A delegate object that responds when people interact with items that the data scanner recognizes.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
protocol DataScannerViewControllerDelegate : AnyObject
```

## Mentioned in 

Scanning data with the camera

## Overview

Implement this protocol to handle when people tap recognized items and, optionally, provide additional feedback when the data scanner updates the recognized items.

## Topics

### Customizing highlighting

func dataScanner(DataScannerViewController, didAdd: [RecognizedItem], allItems: [RecognizedItem])

Responds when the data scanner starts recognizing an item.

**Required** Default implementation provided.

func dataScanner(DataScannerViewController, didUpdate: [RecognizedItem], allItems: [RecognizedItem])

Responds when the data scanner updates the geometry of an item it recognizes.

**Required** Default implementation provided.

func dataScanner(DataScannerViewController, didRemove: [RecognizedItem], allItems: [RecognizedItem])

Responds when the data scanner stops recognizing an item.

**Required** Default implementation provided.

### Zooming

func dataScannerDidZoom(DataScannerViewController)

Responds when a person or your code changes the zoom factor.

**Required** Default implementation provided.

### Tapping items

func dataScanner(DataScannerViewController, didTapOn: RecognizedItem)

Responds when a person taps an item that the data scanner recognizes.

**Required** Default implementation provided.

### Handling errors

func dataScanner(DataScannerViewController, becameUnavailableWithError: DataScannerViewController.ScanningUnavailable)

Responds when the data scanner becomes unavailable and stops scanning.

**Required** Default implementation provided.

## See Also

### Barcode and text scanning through the camera

Scanning data with the camera

Enable Live Text data scanning of text and codes that appear in the camera’s viewfinder.

class DataScannerViewController

An object that scans the camera live video for text, data in text, and machine-readable codes.

enum RecognizedItem

An item that the data scanner recognizes in the camera’s live video.

