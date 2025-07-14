

- Media Library
- MLMediaGroup
-  url 

Instance Property

# url

The location of the media group.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
var url: URL? { get }
```

## Discussion

Some groups do not have a URL, in which case this returns `nil`. For example, a group that represents a filesystem folder on disk has a URL, but a group that represents a named face in iPhoto does not.

## See Also

### Accessing Group Attributes

var attributes: [String : Any]

A dictionary of attributes describing the media group.

var name: String?

The name of the media group.

var iconImage: NSImage?

The media group’s icon.

var modificationDate: Date?

The date and time when the media group was last altered.

