

- VisionKit
- DataScannerViewControllerDelegate
-  dataScannerDidZoom(\_:) 

Instance Method

# dataScannerDidZoom(\_:)

Responds when a person or your code changes the zoom factor.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
func dataScannerDidZoom(_ dataScanner: DataScannerViewController)
```

**Required** Default implementation provided.

## Parameters 

`dataScanner`  

The data scanner whose zoom factor changes.

## Discussion

The data scanner invokes this method when the zoomFactor property changes.

## Default Implementations

### DataScannerViewControllerDelegate Implementations

func dataScannerDidZoom(DataScannerViewController)

A default, blank implementation for when a person or your code changes the zoom factor.

