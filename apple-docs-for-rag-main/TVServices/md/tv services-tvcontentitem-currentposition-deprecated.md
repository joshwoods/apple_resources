

- TV Services
- TVContentItem
-  currentPosition Deprecated

Instance Property

# currentPosition

The index location, measured in seconds, at which the user last played this item.

tvOS 9.0–13.0Deprecated

``` source
@NSCopying
var currentPosition: NSNumber? { get set }
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Discussion

The number is interpreted as a double number of seconds.

## See Also

### Inspecting the Playback Properties

var hasPlayedToEnd: NSNumber?

A Boolean value indicating whether the user can be considered to have finished this item.

Deprecated

var lastAccessedDate: Date?

The date when the user last accessed this item.

Deprecated

