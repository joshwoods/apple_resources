

- AppKit
- NSTextAttachment
-  init(fileWrapper:) 

Initializer

# init(fileWrapper:)

Creates a text attachment object to contain the specified file wrapper.

macOS 10.0+

``` source
convenience init(fileWrapper: FileWrapper?)
```

## Parameters 

`fileWrapper`  

The file wrapper for the attachment.

## Return Value

A new text attachment object initialized with the file wrapper.

## Discussion

This method is the designated initializer for the NSTextAttachment class in macOS.

If `aWrapper` contains an image file that the receiver can interpret as an NSImage object, this method sets the attachment cell’s image to that image rather than to the icon of `aWrapper`.

## See Also

### Initializing a text attachment

init(data: Data?, ofType: String?)

Creates a text attachment object with the specified data.

