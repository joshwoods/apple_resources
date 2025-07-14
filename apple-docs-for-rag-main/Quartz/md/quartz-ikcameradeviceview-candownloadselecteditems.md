

- Quartz
- IKCameraDeviceView
-  canDownloadSelectedItems 

Instance Property

# canDownloadSelectedItems

Returns whether the selected items can be downloaded

macOS 10.6+

``` source
@MainActor
var canDownloadSelectedItems: Bool { get }
```

## See Also

### Configuring Download Interface and Downloading Files

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

var displaysDownloadsDirectoryControl: Bool

Specifies whether the downloads directory control should be displayed.

