

- TV Services
- TVContentItem
-  imageShape Deprecated

Instance Property

# imageShape

The intended aspect ratio or shape of the content image.

tvOS 9.0–13.0Deprecated

``` source
var imageShape: TVContentItemImageShape { get set }
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Discussion

When the TV Content object is being used to represent Top Shelf items, then the allowed values for this property depend on the topShelfStyle property of the object that implements the TV TopShelf extension. For more information, see TVTopShelfProvider.

If the topShelfStyle value is TVTopShelfContentStyle.inset, the valid values of this property are:

- TVContentItemImageShape.extraWide

If the topShelfStyle value is TVTopShelfContentStyle.sectioned, the valid values are:

- TVContentItemImageShape.poster

- TVContentItemImageShape.square

- TVContentItemImageShape.HDTV

If the value of this property is not valid for the current Top Shelf style, the system reserves the right to scale the image in any way.

## See Also

### Inspecting the Content Properties

var creationDate: Date?

The date when the content item was created, or the date when it was first broadcast, or some other kind of origination date.

Deprecated

var duration: NSNumber?

The amount of time required to play the media to completion.

Deprecated

var expirationDate: Date?

The date when the user will no longer be able to access the item.

Deprecated

enum TVContentItemImageShape

An enumerated type that identifies the shape in which the content item should be displayed.

