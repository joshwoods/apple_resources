

- TV Services
- TVContentItem
-  duration Deprecated

Instance Property

# duration

The amount of time required to play the media to completion.

tvOS 9.0–13.0Deprecated

``` source
@NSCopying
var duration: NSNumber? { get set }
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Discussion

The duration number is interpreted as a double number of seconds.

## See Also

### Inspecting the Content Properties

var creationDate: Date?

The date when the content item was created, or the date when it was first broadcast, or some other kind of origination date.

Deprecated

var expirationDate: Date?

The date when the user will no longer be able to access the item.

Deprecated

var imageShape: TVContentItemImageShape

The intended aspect ratio or shape of the content image.

Deprecated

enum TVContentItemImageShape

An enumerated type that identifies the shape in which the content item should be displayed.

