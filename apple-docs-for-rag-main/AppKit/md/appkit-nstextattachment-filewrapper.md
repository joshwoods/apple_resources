

- AppKit
- NSTextAttachment
-  fileWrapper 

Instance Property

# fileWrapper

The text attachment’s file wrapper.

macOS 10.0+

``` source
var fileWrapper: FileWrapper? { get set }
```

## Discussion

The file wrapper holds the contents of the attached file. In iOS, modifying this property has a side effect of invalidating the image, contents, and fileType properties.

## See Also

### Defining the attachment’s contents

var bounds: CGRect

The layout bounds of the text attachment’s graphical representation in the text coordinate system.

var contents: Data?

The contents for the text attachment.

var fileType: String?

The file type of the contents for the text attachment.

var image: NSImage?

An instance of the relevant image class that represents the contents of the text attachment object.

var allowsTextAttachmentView: Bool

A Boolean value that determines whether the text attachment uses text attachment views.

var usesTextAttachmentView: Bool

A Boolean value that indicates whether the text attachment uses text attachment views.

var lineLayoutPadding: CGFloat

The layout padding before and after the text attachment bounds.

