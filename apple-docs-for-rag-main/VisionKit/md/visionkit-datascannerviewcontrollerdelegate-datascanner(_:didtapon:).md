

- VisionKit
- DataScannerViewControllerDelegate
-  dataScanner(\_:didTapOn:) 

Instance Method

# dataScanner(\_:didTapOn:)

Responds when a person taps an item that the data scanner recognizes.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
func dataScanner(
    _ dataScanner: DataScannerViewController,
    didTapOn item: RecognizedItem
)
```

**Required** Default implementation provided.

## Parameters 

`dataScanner`  

The data scanner with the zoom factor that changes.

`item`  

The item that a person taps.

## Mentioned in 

Scanning data with the camera

## Discussion

Implement this method to take some action, depending on the type of data that a person taps.

## Default Implementations

### DataScannerViewControllerDelegate Implementations

func dataScanner(DataScannerViewController, didTapOn: RecognizedItem)

A default, blank implementation for when a person taps an item that the data scanner recognizes.

