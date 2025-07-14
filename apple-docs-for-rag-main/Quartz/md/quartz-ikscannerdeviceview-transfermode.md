

- Quartz
- IKScannerDeviceView
-  transferMode 

Instance Property

# transferMode

Determines how the scanned content is provided to the delegate.

macOS 10.6+

``` source
@MainActor
var transferMode: IKScannerDeviceViewTransferMode { get set }
```

## Discussion

The supported constants are defined in IKScannerDeviceViewTransferMode.

## See Also

### Configuring Downloading

var displaysDownloadsDirectoryControl: Bool

Determines whether the downloads directory control is displayed.

var downloadsDirectory: URL!

The directory where scans are saved.

var documentName: String!

Returns the document name.

