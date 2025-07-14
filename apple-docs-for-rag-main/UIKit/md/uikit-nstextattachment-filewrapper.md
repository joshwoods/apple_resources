

- UIKit
- NSTextAttachment
-  fileWrapper 

Instance Property

# fileWrapper

The text attachment’s file wrapper.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

var image: UIImage?

An instance of the relevant image class that represents the contents of the text attachment object.

var allowsTextAttachmentView: Bool

A Boolean value that determines whether the text attachment uses text attachment views.

var usesTextAttachmentView: Bool

A Boolean value that indicates whether the text attachment uses text attachment views.

var lineLayoutPadding: CGFloat

The layout padding before and after the text attachment bounds.

