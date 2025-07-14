

- Quartz
- IKScannerDeviceView
-  downloadsDirectory 

Instance Property

# downloadsDirectory

The directory where scans are saved.

macOS 10.6+

``` source
@MainActor
var downloadsDirectory: URL! { get set }
```

## See Also

### Configuring Downloading

var displaysDownloadsDirectoryControl: Bool

Determines whether the downloads directory control is displayed.

var transferMode: IKScannerDeviceViewTransferMode

Determines how the scanned content is provided to the delegate.

var documentName: String!

Returns the document name.

