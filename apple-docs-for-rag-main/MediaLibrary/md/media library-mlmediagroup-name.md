

- Media Library
- MLMediaGroup
-  name 

Instance Property

# name

The name of the media group.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
var name: String? { get }
```

## Discussion

This string is human-readable. It is either user created (such as the name of an iTunes playlist) or already localized.

## See Also

### Accessing Group Attributes

var attributes: [String : Any]

A dictionary of attributes describing the media group.

var iconImage: NSImage?

The media group’s icon.

var url: URL?

The location of the media group.

var modificationDate: Date?

The date and time when the media group was last altered.

