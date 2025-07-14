

- Core Spotlight
- CSSearchableItemAttributeSet
-  contentSources 

Instance Property

# contentSources

An array of sources from which the media was obtained.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var contentSources: [String]? { get set }
```

## Discussion

The string values in this property might include the URL of the website from which the file was downloaded or information that describes the email to which the file was attached.

## See Also

### Describing media

var comment: String?

A comment related to the media file.

var contentCreationDate: Date?

The creation date of an edited or optimized version of the song or composition.

var contentModificationDate: Date?

The date on which the contents of the file was last modified.

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

var mediaTypes: [String]?

The media types present in the content.

