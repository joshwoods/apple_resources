

- TV Services
- TVContentItem
-  lastAccessedDate Deprecated

Instance Property

# lastAccessedDate

The date when the user last accessed this item.

tvOS 9.0–13.0Deprecated

``` source
var lastAccessedDate: Date? { get set }
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Discussion

A typical use is for content types in which “playing” represents the date when the user last played the item or played a subitem within the group. When the user simply looks at an item, the access date should not change.

## See Also

### Inspecting the Playback Properties

var currentPosition: NSNumber?

The index location, measured in seconds, at which the user last played this item.

Deprecated

var hasPlayedToEnd: NSNumber?

A Boolean value indicating whether the user can be considered to have finished this item.

Deprecated

