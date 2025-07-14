

- AppKit
- NSTextAttachment
-  image 

Instance Property

# image

An instance of the relevant image class that represents the contents of the text attachment object.

macOS 10.11+

``` source
var image: NSImage? { get set }
```

## Discussion

For details about using the UIImage class to create text attachments that automatically adjust to surrounding font and color attributes, see the doc://com.apple.documentation/documentation/uikit/nstextattachment/3327290-init initializer.

## See Also

### Defining the attachment’s contents

var bounds: CGRect

The layout bounds of the text attachment’s graphical representation in the text coordinate system.

var contents: Data?

The contents for the text attachment.

var fileType: String?

The file type of the contents for the text attachment.

var fileWrapper: FileWrapper?

The text attachment’s file wrapper.

var allowsTextAttachmentView: Bool

A Boolean value that determines whether the text attachment uses text attachment views.

var usesTextAttachmentView: Bool

A Boolean value that indicates whether the text attachment uses text attachment views.

var lineLayoutPadding: CGFloat

The layout padding before and after the text attachment bounds.

