

- Quartz
- IKScannerDeviceView
-  displaysDownloadsDirectoryControl 

Instance Property

# displaysDownloadsDirectoryControl

Determines whether the downloads directory control is displayed.

macOS 10.6+

``` source
@MainActor
var displaysDownloadsDirectoryControl: Bool { get set }
```

## See Also

### Configuring Downloading

var downloadsDirectory: URL!

The directory where scans are saved.

var transferMode: IKScannerDeviceViewTransferMode

Determines how the scanned content is provided to the delegate.

var documentName: String!

Returns the document name.

