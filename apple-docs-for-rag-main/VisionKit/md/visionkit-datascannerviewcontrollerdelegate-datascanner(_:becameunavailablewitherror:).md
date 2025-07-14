

- VisionKit
- DataScannerViewControllerDelegate
-  dataScanner(\_:becameUnavailableWithError:) 

Instance Method

# dataScanner(\_:becameUnavailableWithError:)

Responds when the data scanner becomes unavailable and stops scanning.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
func dataScanner(
    _ dataScanner: DataScannerViewController,
    becameUnavailableWithError error: DataScannerViewController.ScanningUnavailable
)
```

**Required** Default implementation provided.

## Parameters 

`dataScanner`  

The data scanner that’s not available.

`error`  

Describes an error if it occurs.

## Mentioned in 

Scanning data with the camera

## Default Implementations

### DataScannerViewControllerDelegate Implementations

func dataScanner(DataScannerViewController, becameUnavailableWithError: DataScannerViewController.ScanningUnavailable)

A default, blank implementation for when the data scanner becomes unavailable and stops scanning.

