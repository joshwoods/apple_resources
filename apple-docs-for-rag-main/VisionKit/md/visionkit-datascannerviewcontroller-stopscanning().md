

- VisionKit
- DataScannerViewController
-  stopScanning() 

Instance Method

# stopScanning()

Stops scanning the camera’s live video for data.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
func stopScanning()
```

## Mentioned in 

Scanning data with the camera

## Discussion

This method removes all items from the recognizedItems property.

## See Also

### Scanning and recognizing items

func startScanning() throws

Starts scanning the camera’s live video for data.

var isScanning: Bool

A Boolean value that indicates whether the data scanner is actively looking for items.

var recognizedItems: AsyncStream&lt;[RecognizedItem]>

An asynchronous array of items that the data scanner currently recognizes in the camera’s live video.

