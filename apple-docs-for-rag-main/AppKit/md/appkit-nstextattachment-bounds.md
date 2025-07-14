

- AppKit
- NSTextAttachment
-  bounds 

Instance Property

# bounds

The layout bounds of the text attachment’s graphical representation in the text coordinate system.

macOS 10.11+

``` source
var bounds: CGRect { get set }
```

## Discussion

The bounds rectangle origin is at the current glyph location on the text baseline. The default value is CGRectZero.

## See Also

### Defining the attachment’s contents

var contents: Data?

The contents for the text attachment.

var fileType: String?

The file type of the contents for the text attachment.

var image: NSImage?

An instance of the relevant image class that represents the contents of the text attachment object.

var fileWrapper: FileWrapper?

The text attachment’s file wrapper.

var allowsTextAttachmentView: Bool

A Boolean value that determines whether the text attachment uses text attachment views.

var usesTextAttachmentView: Bool

A Boolean value that indicates whether the text attachment uses text attachment views.

var lineLayoutPadding: CGFloat

The layout padding before and after the text attachment bounds.

