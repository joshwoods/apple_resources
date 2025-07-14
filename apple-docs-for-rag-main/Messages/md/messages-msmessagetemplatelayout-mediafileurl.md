

- Messages
- MSMessageTemplateLayout
-  mediaFileURL 

Instance Property

# mediaFileURL

A media file used to represent the message in the transcript.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var mediaFileURL: URL? { get set }
```

## Discussion

The media file URL must be a file URL. For video files, the system crops the left and right edges of the media file by 6 points, and rounds its corners. For audio files, it shows a graphical representation of the audio’s waveform.

The template can have either an image or a media file. This property is ignored if the template has a non-`nil` image property. This property defaults to `nil`.

## See Also

### Assigning Visual Elements

var image: UIImage?

An image used to represent the message in the transcript.

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

