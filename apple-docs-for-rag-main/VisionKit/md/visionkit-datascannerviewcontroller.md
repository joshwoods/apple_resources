

- VisionKit
-  DataScannerViewController 

Class

# DataScannerViewController

An object that scans the camera live video for text, data in text, and machine-readable codes.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor @objc
class DataScannerViewController
```

## Mentioned in 

Scanning data with the camera

## Overview

Use a `DataScannerViewController` object to get input from physical objects that appear in the camera’s live video, such as printed text and QR codes on packages.

Create a data scanner by passing parameters that configure the interface to the init(recognizedDataTypes:qualityLevel:recognizesMultipleItems:isHighFrameRateTrackingEnabled:isPinchToZoomEnabled:isGuidanceEnabled:isHighlightingEnabled:) initializer. Then set its delegate to an object in your app that implements the DataScannerViewControllerDelegate protocol.

Before presenting the view controller, check whether the data scanner is available using the isSupported and isAvailable properties. Before you can use the data scanner, you must provide a reason for using the camera (add the NSCameraUsageDescription key to the information property list), and a person must agree when the system dialog first appears.

Then begin data scanning by invoking the startScanning() method and implement the dataScanner(_:didTapOn:) and similar delegate methods to handle user actions. Use the RecognizedItem parameter passed to these methods to perform data-specific actions. For example, if the item is a QR code, perform an action with its payload string, such as opening a URL in a browser, or calling a phone number.

Alternatively, you can track items that appear in the live video using the asynchronous recognizedItems array.

## Topics

### Handling availability

class var isSupported: Bool

A Boolean value that indicates whether the device supports data scanning.

class var isAvailable: Bool

A Boolean value that indicates whether a person grants your app access to the camera and doesn’t have any restrictions to using the camera.

class var supportedTextRecognitionLanguages: [String]

The identifiers for the languages that the data scanner recognizes.

enum ScanningUnavailable

The possible reasons the data scanner is unavailable.

### Creating data scanners

init(recognizedDataTypes: Set&lt;DataScannerViewController.RecognizedDataType>, qualityLevel: DataScannerViewController.QualityLevel, recognizesMultipleItems: Bool, isHighFrameRateTrackingEnabled: Bool, isPinchToZoomEnabled: Bool, isGuidanceEnabled: Bool, isHighlightingEnabled: Bool)

Creates a scanner for finding data, such as text and machine-readable codes, in the camera’s live video.

let recognizedDataTypes: Set&lt;DataScannerViewController.RecognizedDataType>

The types of data that the data scanner identifies in the live video.

struct RecognizedDataType

A type of data that the scanner recognizes.

### Configuring data scanners

var delegate: (any DataScannerViewControllerDelegate)?

The delegate that handles user interaction with items recognized by the data scanner.

let qualityLevel: DataScannerViewController.QualityLevel

The resolution that the scanner uses to find data.

enum QualityLevel

The possible quality levels that the scanner uses to find data.

let recognizesMultipleItems: Bool

A Boolean value that indicates whether the scanner should identify all items in the live video.

let isHighFrameRateTrackingEnabled: Bool

A Boolean value that determines the frequency at which the scanner updates the geometry of recognized items.

let isPinchToZoomEnabled: Bool

A Boolean value that indicates whether people can use a two-finger pinch-to-zoom gesture.

let isGuidanceEnabled: Bool

A Boolean value that indicates whether the scanner provides help to a person when selecting items.

let isHighlightingEnabled: Bool

A Boolean value that indicates whether the scanner displays highlights around recognized items.

### Zooming

var zoomFactor: Double

The zoom factor for the live video in the camera.

var minZoomFactor: Double

The minimum zoom factor that the camera supports.

var maxZoomFactor: Double

The maximum zoom factor that the camera supports.

### Scanning and recognizing items

func startScanning() throws

Starts scanning the camera’s live video for data.

func stopScanning()

Stops scanning the camera’s live video for data.

var isScanning: Bool

A Boolean value that indicates whether the data scanner is actively looking for items.

var recognizedItems: AsyncStream&lt;[RecognizedItem]>

An asynchronous array of items that the data scanner currently recognizes in the camera’s live video.

### Capturing photos

func capturePhoto() async throws -> UIImage

Captures a high-resolution photo of the camera’s live video.

### Customizing the interface

var overlayContainerView: UIView

A view that the data scanner displays over its view without interfering with the Live Text interface.

var regionOfInterest: CGRect?

The area of the live video in view coordinates that the data scanner searches for items.

### Responding to view controller events

func loadView()

Creates the view that the controller manages.

func viewDidLoad()

Performs some action after the system loads the view into memory.

func viewWillAppear(Bool)

Performs some action before the view appears.

func viewDidDisappear(Bool)

Performs some action after the view disappears.

func removeFromParent()

Removes the view controller from its parent.

### Enumerations

enum TextContentType

Types of text that a data scanner recognizes.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Barcode and text scanning through the camera

Scanning data with the camera

Enable Live Text data scanning of text and codes that appear in the camera’s viewfinder.

protocol DataScannerViewControllerDelegate

A delegate object that responds when people interact with items that the data scanner recognizes.

enum RecognizedItem

An item that the data scanner recognizes in the camera’s live video.

