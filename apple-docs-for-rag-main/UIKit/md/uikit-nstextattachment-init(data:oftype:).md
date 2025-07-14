

- UIKit
- NSTextAttachment
-  init(data:ofType:) 

Initializer

# init(data:ofType:)

Creates a text attachment object with the specified data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    data contentData: Data?,
    ofType uti: String?
)
```

## Parameters 

`contentData`  

Data to use for the text attachment contents. Can be `nil`.

`uti`  

A uniform type identifier specifying the data type of the attachment contents. Can be `nil`.

## Return Value

A new `NSTextAttachment` object.

## Discussion

This method is the designated initializer for the `NSTextAttachment` class on iOS.

When either `contentData` or `uti` is `nil`, TextKit considers the receiver to be an attachment without document contents. In this case, the `NSAttributedString` external file writing methods try to save the value of the image property instead.

## See Also

### Initializing a text attachment

convenience init(fileWrapper: FileWrapper?)

Creates a text attachment object to contain the specified file wrapper.

init(image: UIImage)

Creates a text attachment object to contain the specified image.

