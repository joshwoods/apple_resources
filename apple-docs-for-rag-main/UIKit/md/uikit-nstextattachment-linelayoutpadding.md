

- UIKit
- NSTextAttachment
-  lineLayoutPadding 

Instance Property

# lineLayoutPadding

The layout padding before and after the text attachment bounds.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var lineLayoutPadding: CGFloat { get set }
```

## Discussion

The layout and rendering bounds X origin is inset by the padding value. This affects the relationship between the text attachment bounds and `NSLayoutManager` glyph metrics methods location(forGlyphAt:) and attachmentSize(forGlyphAt:). The default value is `0.0`.

## See Also

### Defining the attachment’s contents

var bounds: CGRect

The layout bounds of the text attachment’s graphical representation in the text coordinate system.

var contents: Data?

The contents for the text attachment.

var fileType: String?

The file type of the contents for the text attachment.

var image: UIImage?

An instance of the relevant image class that represents the contents of the text attachment object.

var fileWrapper: FileWrapper?

The text attachment’s file wrapper.

var allowsTextAttachmentView: Bool

A Boolean value that determines whether the text attachment uses text attachment views.

var usesTextAttachmentView: Bool

A Boolean value that indicates whether the text attachment uses text attachment views.

