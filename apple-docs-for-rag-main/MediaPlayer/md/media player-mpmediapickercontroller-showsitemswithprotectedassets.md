

- Media Player
- MPMediaPickerController
-  showsItemsWithProtectedAssets 

Instance Property

# showsItemsWithProtectedAssets

A Boolean value that specifies whether the media item picker displays protected assets.

iOS 9.2+iPadOS 9.2+Mac Catalyst 13.1+

``` source
@MainActor
var showsItemsWithProtectedAssets: Bool { get set }
```

## Discussion

When set to true, the media item picker displays media items with DRM. The default value for this property is true.

## See Also

### Using a media item picker

var allowsPickingMultipleItems: Bool

A Boolean value specifying the default selection behavior for a media item picker.

var showsCloudItems: Bool

A Boolean value specifying whether to display iCloud Media Library items for a media picker.

var mediaTypes: MPMediaType

The media types that media item picker presents.

var prompt: String?

A prompt, for the user, that appears above the navigation bar buttons.

