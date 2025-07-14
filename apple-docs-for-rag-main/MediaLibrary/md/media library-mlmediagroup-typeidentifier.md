

- Media Library
- MLMediaGroup
-  typeIdentifier 

Instance Property

# typeIdentifier

An identifier for the media group’s type.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
var typeIdentifier: String { get }
```

## Discussion

Multiple groups within a media source can have the same type identifier. For descriptions of group type identifiers, see MediaLibrary Constants.

## See Also

### Identifying the Group

var identifier: String

An identifier for the media group.

var mediaSourceIdentifier: String

An identifier for the source that loaded the media group.

var mediaLibrary: MLMediaLibrary?

A pointer to the media library instance that loaded the media group’s source.

