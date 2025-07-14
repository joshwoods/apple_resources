

- TV Services
-  TVContentItemImageShape 

Enumeration

# TVContentItemImageShape

An enumerated type that identifies the shape in which the content item should be displayed.

tvOS 9.0+

``` source
enum TVContentItemImageShape
```

## Topics

### Constants

case none

The content has no particular shape.

case poster

The content has a width:height ratio of `2:3`.

case square

The content has a width:height ratio of `1:1`.

case SDTV

The content is standard-definition television content with a width:height ratio of `4:3`.

case HDTV

The content is high-definition television content with a width:height ratio of `16:9`.

case wide

The content has a width:height ratio of `8:3`.

case extraWide

The content has a width:height ratio of `80:27`.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var imageShape: TVContentItemImageShape

The intended aspect ratio or shape of the content image.

Deprecated

