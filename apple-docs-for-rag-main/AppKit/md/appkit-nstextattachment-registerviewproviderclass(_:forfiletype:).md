

- AppKit
- NSTextAttachment
-  registerViewProviderClass(\_:forFileType:) 

Type Method

# registerViewProviderClass(\_:forFileType:)

Registers a specific file type with the attachment view provider.

macOS 12.0+

``` source
class func registerViewProviderClass(
    _ textAttachmentViewProviderClass: AnyClass,
    forFileType fileType: String
)
```

## Parameters 

`textAttachmentViewProviderClass`  

The text attachment view provider class.

`fileType`  

A String that represents the file type.

## See Also

### Convenience methods

class func textAttachmentViewProviderClass(forFileType: String) -> AnyClass?

Returns the text attachment view provider class, if any, for the file type you specify.

