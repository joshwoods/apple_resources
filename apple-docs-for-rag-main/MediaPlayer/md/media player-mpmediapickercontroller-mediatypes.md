

- Media Player
- MPMediaPickerController
-  mediaTypes 

Instance Property

# mediaTypes

The media types that media item picker presents.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+

``` source
@MainActor
var mediaTypes: MPMediaType { get }
```

## Discussion

MPMediaType lists the available media types.

## See Also

### Using a media item picker

var allowsPickingMultipleItems: Bool

A Boolean value specifying the default selection behavior for a media item picker.

var showsCloudItems: Bool

A Boolean value specifying whether to display iCloud Media Library items for a media picker.

var prompt: String?

A prompt, for the user, that appears above the navigation bar buttons.

var showsItemsWithProtectedAssets: Bool

A Boolean value that specifies whether the media item picker displays protected assets.

