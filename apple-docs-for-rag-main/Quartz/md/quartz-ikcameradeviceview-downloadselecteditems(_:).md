

- Quartz
- IKCameraDeviceView
-  downloadSelectedItems(\_:) 

Instance Method

# downloadSelectedItems(\_:)

Deletes the selected items from the camera.

macOS 10.6+

``` source
@IBAction @MainActor
func downloadSelectedItems(_ sender: Any!)
```

## Parameters 

`sender`  

The object that sent the message.

## Discussion

This method is can be connected to a user interface item in Interface Builder.

## See Also

### Configuring Download Interface and Downloading Files

var canDownloadSelectedItems: Bool

Returns whether the selected items can be downloaded

var downloadsDirectory: URL!

Specifies the directory where files are downloaded

func downloadAllItems(Any!)

Downloads all the items.

var downloadSelectedControlLabel: String!

Allows the “Download Selected” control to be renamed.

var downloadAllControlLabel: String!

Allows the “Download All” control to be renamed.

var displaysDownloadsDirectoryControl: Bool

Specifies whether the downloads directory control should be displayed.

