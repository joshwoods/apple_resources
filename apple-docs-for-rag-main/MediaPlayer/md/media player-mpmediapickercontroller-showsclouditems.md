

- Media Player
- MPMediaPickerController
-  showsCloudItems 

Instance Property

# showsCloudItems

A Boolean value specifying whether to display iCloud Media Library items for a media picker.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
var showsCloudItems: Bool { get set }
```

## Discussion

When set to true, the picker shows available iCloud Music Library items, including purchased items, imported content, and Apple Music subscription content. When set to false, the picker only shows content downloaded to the device. The default value is true.

## See Also

### Using a media item picker

var allowsPickingMultipleItems: Bool

A Boolean value specifying the default selection behavior for a media item picker.

var mediaTypes: MPMediaType

The media types that media item picker presents.

var prompt: String?

A prompt, for the user, that appears above the navigation bar buttons.

var showsItemsWithProtectedAssets: Bool

A Boolean value that specifies whether the media item picker displays protected assets.

