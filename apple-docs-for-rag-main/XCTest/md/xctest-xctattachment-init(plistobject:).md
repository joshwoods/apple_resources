

- XCTest
- XCTAttachment
-  init(plistObject:) 

Initializer

# init(plistObject:)

Creates an attachment from an object that can be represented in an XML property list.

``` source
convenience init(plistObject object: Any)
```

## Parameters 

`object`  

An object that can be serialized to an XML property list format, such as an array, dictionary, string, or date.

## Discussion

The content of the attachment is an XML property list representation of the provided object with a uniformTypeIdentifier value of `"com.apple.xml-property-list"`.

Note

Creating an attachment with a non-property-list-compatible object will trigger an exception at the point that the attachment is added to an XCTActivity.

## See Also

### Creating Attachments from Objects

convenience init(archivableObject: any NSSecureCoding)

Creates an attachment from an object that conforms to `NSSecureCoding`.

convenience init(archivableObject: any NSSecureCoding, uniformTypeIdentifier: String)

Creates an attachment from an object that conforms to `NSSecureCoding`, with a custom UTI.

