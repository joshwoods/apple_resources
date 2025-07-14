

- Media Player
- MPMediaPickerController
-  allowsPickingMultipleItems 

Instance Property

# allowsPickingMultipleItems

A Boolean value specifying the default selection behavior for a media item picker.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+

``` source
@MainActor
var allowsPickingMultipleItems: Bool { get set }
```

## Discussion

When set to true, the media item picker allows the selection of multiple media items. When set to false, the media picker only allows the selection of a single media item. The label for the button that dismisses the picker is “Done” when this value is true and “Cancel” when it’s false.

## See Also

### Using a media item picker

var showsCloudItems: Bool

A Boolean value specifying whether to display iCloud Media Library items for a media picker.

var mediaTypes: MPMediaType

The media types that media item picker presents.

var prompt: String?

A prompt, for the user, that appears above the navigation bar buttons.

var showsItemsWithProtectedAssets: Bool

A Boolean value that specifies whether the media item picker displays protected assets.

