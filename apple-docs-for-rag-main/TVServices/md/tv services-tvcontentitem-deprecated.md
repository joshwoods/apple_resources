

- TV Services
-  TVContentItem Deprecated

Class

# TVContentItem

An object that describes either a piece of content or a container for other content items.

tvOS 9.0–13.0Deprecated

``` source
class TVContentItem
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Overview

The exact details of what a content item is are dependent on your app. For example, a content item might be a piece of media or it might provide access to news or other content available to your app.

To create a description of a piece of content, create a content identifier object and then use this object to initialize a new TVContentItem object. Then, set any other properties that are appropriate for the object you are creating. Most of the properties are optional, and many properties apply only to certain kinds of content. Inspect an existing TVContentItem object to retrieve the media and playback properties, such as the duration of the content or when the content was last played.

## Topics

### Initializing a Content Item

init(contentIdentifier: TVContentIdentifier)

Initializes a new content item.

init?(coder: NSCoder)

Returns an object initialized from data in a given unarchiver.

### Reading a Content Item’s Identifier

var contentIdentifier: TVContentIdentifier

The content identifier that uniquely identifies this item.

### Inspecting the General Display Properties

These properties describe the item to be displayed..

var badgeCount: NSNumber?

A badging integer for this item.

var title: String?

The localized string title of the item.

var topShelfItems: [TVContentItem]?

An array of content items that are the items of a section.

### Accessing Image Resources

var imageURL: URL?

A URL giving the location of the image to be displayed for this content item.

func imageURL(forTraits: TVContentItemImageTrait) -> URL?

Retrieve the URL for the image that best matches the specified traits.

func setImageURL(URL?, forTraits: TVContentItemImageTrait)

struct TVContentItemImageTrait

Traits describing the type of image you want.

### Inspecting the Content Properties

These properties are used to describe the underlying content item.

var creationDate: Date?

The date when the content item was created, or the date when it was first broadcast, or some other kind of origination date.

var duration: NSNumber?

The amount of time required to play the media to completion.

var expirationDate: Date?

The date when the user will no longer be able to access the item.

var imageShape: TVContentItemImageShape

The intended aspect ratio or shape of the content image.

enum TVContentItemImageShape

An enumerated type that identifies the shape in which the content item should be displayed.

### Inspecting the Playback Properties

var currentPosition: NSNumber?

The index location, measured in seconds, at which the user last played this item.

var hasPlayedToEnd: NSNumber?

A Boolean value indicating whether the user can be considered to have finished this item.

var lastAccessedDate: Date?

The date when the user last accessed this item.

### Inspecting the Application Launch Properties

The application launch properties are URLs that the system can use to launch your app. Each URL specifies the content item to be launched and the action to be taken. You are responsible for creating a URL scheme and adding code to your app so that it can respond when these URLs are invoked.

var displayURL: URL?

A URL that causes the app which created this content item to display a description screen for the item.

var playURL: URL?

A URL that causes the app which created this content item to begin playing the item at the user’s current position.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Content

class TVContentIdentifier

An object that uniquely identifies media content in either a single piece or a collection.

Deprecated

func TVTopShelfImageSize(shape: TVContentItemImageShape, style: TVTopShelfContentStyle) -> CGSize

Returns the ideal size for an image, according to its particular shape and style.

Deprecated

