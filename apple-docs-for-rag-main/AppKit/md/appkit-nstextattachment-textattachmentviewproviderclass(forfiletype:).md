

- AppKit
- NSTextAttachment
-  textAttachmentViewProviderClass(forFileType:) 

Type Method

# textAttachmentViewProviderClass(forFileType:)

Returns the text attachment view provider class, if any, for the file type you specify.

macOS 12.0+

``` source
class func textAttachmentViewProviderClass(forFileType fileType: String) -> AnyClass?
```

## Parameters 

`fileType`  

A String that represents the file type.

## Return Value

The text attachment view provider class, or `nil` if the there is no class for the specified file type.

## See Also

### Convenience methods

class func registerViewProviderClass(AnyClass, forFileType: String)

Registers a specific file type with the attachment view provider.

