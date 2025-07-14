

- Quartz
- IKCameraDeviceView
-  downloadAllItems(\_:) 

Instance Method

# downloadAllItems(\_:)

Downloads all the items.

macOS 10.6+

``` source
@IBAction @MainActor
func downloadAllItems(_ sender: Any!)
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

func downloadSelectedItems(Any!)

Deletes the selected items from the camera.

var downloadSelectedControlLabel: String!

Allows the “Download Selected” control to be renamed.

var downloadAllControlLabel: String!

Allows the “Download All” control to be renamed.

var displaysDownloadsDirectoryControl: Bool

Specifies whether the downloads directory control should be displayed.

