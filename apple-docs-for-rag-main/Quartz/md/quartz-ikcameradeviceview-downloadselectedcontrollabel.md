

- Quartz
- IKCameraDeviceView
-  downloadSelectedControlLabel 

Instance Property

# downloadSelectedControlLabel

Allows the “Download Selected” control to be renamed.

macOS 10.6+

``` source
@MainActor
var downloadSelectedControlLabel: String! { get set }
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

var downloadAllControlLabel: String!

Allows the “Download All” control to be renamed.

var displaysDownloadsDirectoryControl: Bool

Specifies whether the downloads directory control should be displayed.

