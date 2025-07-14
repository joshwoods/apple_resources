

- VisionKit
- DataScannerViewController
-  recognizedItems 

Instance Property

# recognizedItems

An asynchronous array of items that the data scanner currently recognizes in the camera’s live video.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
var recognizedItems: AsyncStream { get }
```

## Discussion

You can use this property instead of the DataScannerViewControllerDelegate protocol methods to track the recognized items in real time. To get the changes between arrays, use the difference(from:) method. For more information on asynchronous streams, see Concurrency.

Text items in this array appear in the reading order of the language and region.

## See Also

### Scanning and recognizing items

func startScanning() throws

Starts scanning the camera’s live video for data.

func stopScanning()

Stops scanning the camera’s live video for data.

var isScanning: Bool

A Boolean value that indicates whether the data scanner is actively looking for items.

