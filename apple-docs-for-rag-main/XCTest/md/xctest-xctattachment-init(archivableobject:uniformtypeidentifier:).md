

- XCTest
- XCTAttachment
-  init(archivableObject:uniformTypeIdentifier:) 

Initializer

# init(archivableObject:uniformTypeIdentifier:)

Creates an attachment from an object that conforms to `NSSecureCoding`, with a custom UTI.

``` source
convenience init(
    archivableObject object: any NSSecureCoding,
    uniformTypeIdentifier identifier: String
)
```

## Parameters 

`object`  

An encodable object that conforms to NSSecureCoding.

`identifier`  

A custom UTI to represent the encoded data’s type.

## See Also

### Creating Attachments from Objects

convenience init(plistObject: Any)

Creates an attachment from an object that can be represented in an XML property list.

convenience init(archivableObject: any NSSecureCoding)

Creates an attachment from an object that conforms to `NSSecureCoding`.

