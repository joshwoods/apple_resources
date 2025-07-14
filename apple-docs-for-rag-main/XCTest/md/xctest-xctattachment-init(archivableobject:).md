

- XCTest
- XCTAttachment
-  init(archivableObject:) 

Initializer

# init(archivableObject:)

Creates an attachment from an object that conforms to `NSSecureCoding`.

``` source
convenience init(archivableObject object: any NSSecureCoding)
```

## Parameters 

`object`  

An encodable object that conforms to NSSecureCoding.

## Discussion

Creates an attachment with a uniformTypeIdentifier of ``` "``public.data" ```.

## See Also

### Creating Attachments from Objects

convenience init(plistObject: Any)

Creates an attachment from an object that can be represented in an XML property list.

convenience init(archivableObject: any NSSecureCoding, uniformTypeIdentifier: String)

Creates an attachment from an object that conforms to `NSSecureCoding`, with a custom UTI.

