

- Messages
- MSMessageTemplateLayout
-  subcaption 

Instance Property

# subcaption

A left-aligned subcaption for the message bubble.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var subcaption: String? { get set }
```

## Discussion

The subcaption is drawn using gray text, and is positioned below the caption. This property defaults to `nil`.

## See Also

### Assigning Visual Elements

var image: UIImage?

An image used to represent the message in the transcript.

var mediaFileURL: URL?

A media file used to represent the message in the transcript.

var imageTitle: String?

The title for the image or media file.

var imageSubtitle: String?

The subtitle for the image or media file.

var caption: String?

A left-aligned caption for the message bubble.

var trailingCaption: String?

A right-aligned caption for the message bubble.

var trailingSubcaption: String?

A right-aligned subcaption for the message bubble.

