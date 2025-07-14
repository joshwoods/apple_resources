

- Media Library
- MLMediaGroup
-  attributes 

Instance Property

# attributes

A dictionary of attributes describing the media group.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
var attributes: [String : Any] { get }
```

## Discussion

These attributes are usually defined by the source app, such as iTunes. For example, an iTunes playlist is represented as a group. iTunes attaches attributes such as “Playlist Persistent ID” to the group in its `attributes`. The attribute names vary based on the media source. Attributes common to all sources are called out as separate properties.

## See Also

### Accessing Group Attributes

var name: String?

The name of the media group.

var iconImage: NSImage?

The media group’s icon.

var url: URL?

The location of the media group.

var modificationDate: Date?

The date and time when the media group was last altered.

