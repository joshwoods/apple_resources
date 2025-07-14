

- VisionKit
- DataScannerViewController
-  isScanning 

Instance Property

# isScanning

A Boolean value that indicates whether the data scanner is actively looking for items.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
var isScanning: Bool { get }
```

## See Also

### Scanning and recognizing items

func startScanning() throws

Starts scanning the camera’s live video for data.

func stopScanning()

Stops scanning the camera’s live video for data.

var recognizedItems: AsyncStream&lt;[RecognizedItem]>

An asynchronous array of items that the data scanner currently recognizes in the camera’s live video.

