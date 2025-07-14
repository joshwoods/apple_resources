

- TV Services
- TVContentItem
-  hasPlayedToEnd Deprecated

Instance Property

# hasPlayedToEnd

A Boolean value indicating whether the user can be considered to have finished this item.

tvOS 9.0–13.0Deprecated

``` source
@NSCopying
var hasPlayedToEnd: NSNumber? { get set }
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Discussion

The number of this property is interpreted as a Boolean value.

## See Also

### Inspecting the Playback Properties

var currentPosition: NSNumber?

The index location, measured in seconds, at which the user last played this item.

Deprecated

var lastAccessedDate: Date?

The date when the user last accessed this item.

Deprecated

