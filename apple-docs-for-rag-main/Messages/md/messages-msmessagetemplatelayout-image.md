

- Messages
- MSMessageTemplateLayout
-  image 

Instance Property

# image

An image used to represent the message in the transcript.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var image: UIImage? { get set }
```

## Discussion

The system crops the left and right edges of the image by 6 points, and rounds the image’s corners.

The template can have either an image or a media file. If this property is set to a non-`nil` value, the mediaFileURL property is ignored. This property defaults to `nil`.

## See Also

### Assigning Visual Elements

var mediaFileURL: URL?

A media file used to represent the message in the transcript.

var imageTitle: String?

The title for the image or media file.

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

