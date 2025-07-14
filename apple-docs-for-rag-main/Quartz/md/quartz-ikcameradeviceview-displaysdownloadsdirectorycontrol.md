

- Quartz
- IKCameraDeviceView
-  displaysDownloadsDirectoryControl 

Instance Property

# displaysDownloadsDirectoryControl

Specifies whether the downloads directory control should be displayed.

macOS 10.6+

``` source
@MainActor
var displaysDownloadsDirectoryControl: Bool { get set }
```

## See Also

### Configuring Download Interface and Downloading Files

var canDownloadSelectedItems: Bool

Returns whether the selected items can be downloaded

var downloadsDirectory: URL!

Specifies the directory where files are downloaded

func downloadSelectedItems(Any!)

Deletes the selected items from the camera.

func downloadAllItems(Any!)

Downloads all the items.

var downloadSelectedControlLabel: String!

Allows the “Download Selected” control to be renamed.

var downloadAllControlLabel: String!

Allows the “Download All” control to be renamed.

