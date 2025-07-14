

- Core Spotlight
- CSSearchableItemAttributeSet
-  coverage 

Instance Property

# coverage

A list of descriptors that specify the extent or scope of the media.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var coverage: [String]? { get set }
```

## Discussion

The string values in this property typically include a location (such as a place name or geographic coordinates), a temporal period (such as a period label, date, or date range), or a jurisdiction (such as a named administrative entity).

It’s recommended that you select a value from a controlled vocabulary, and that when you need to specify a place or time period, you use a name instead of a numeric identifier, such as a set of coordinates or a date range.

## See Also

### Describing media

var comment: String?

A comment related to the media file.

var contentCreationDate: Date?

The creation date of an edited or optimized version of the song or composition.

var contentModificationDate: Date?

The date on which the contents of the file was last modified.

var contentSources: [String]?

An array of sources from which the media was obtained.

var copyright: String?

The copyright date of the content.

var downloadedDate: Date?

The most recent date on which the file was downloaded or received.

var editors: [String]?

A list of editors who have worked on the file.

var lastUsedDate: Date?

The date on which the file was last used.

var participants: [String]?

A list of people who are visible in an image or movie or written about in a document.

var projects: [String]?

A list of projects of which this file is a part.

var addedDate: Date?

The date on which the item was moved into its current location.

var codecs: [String]?

The codecs used to encode/decode the media.

var contactKeywords: [String]?

A list of contacts who are associated with the content in some way, not including the author.

var deliveryType: NSNumber?

The delivery type of the file.

var duration: NSNumber?

The duration (if appropriate) of the content of the file, in seconds.

