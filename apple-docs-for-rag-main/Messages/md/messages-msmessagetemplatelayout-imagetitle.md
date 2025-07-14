

- Messages
- MSMessageTemplateLayout
-  imageTitle 

Instance Property

# imageTitle

The title for the image or media file.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var imageTitle: String? { get set }
```

## Discussion

The title is drawn using white text on the bottom-left corner of the image or media file. This property defaults to `nil`.

## See Also

### Assigning Visual Elements

var image: UIImage?

An image used to represent the message in the transcript.

var mediaFileURL: URL?

A media file used to represent the message in the transcript.

var imageSubtitle: String?

The subtitle for the image or media file.

var caption: String?

A left-aligned caption for the message bubble.

var subcaption: String?

A left-aligned subcaption for the message bubble.

var trailingCaption: String?

A right-aligned caption for the message bubble.

var trailingSubcaption: String?

A right-aligned subcaption for the message bubble.

