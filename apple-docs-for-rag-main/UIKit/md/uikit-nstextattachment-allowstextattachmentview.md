

- UIKit
- NSTextAttachment
-  allowsTextAttachmentView 

Instance Property

# allowsTextAttachmentView

A Boolean value that determines whether the text attachment uses text attachment views.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var allowsTextAttachmentView: Bool { get set }
```

## Discussion

When `true`, the text attachment tries to use a text attachment view returned by viewProvider(for:location:textContainer:). Default is `true`.

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

var usesTextAttachmentView: Bool

A Boolean value that indicates whether the text attachment uses text attachment views.

var lineLayoutPadding: CGFloat

The layout padding before and after the text attachment bounds.

