

- XCTest
- XCTAttachment
-  userInfo 

Instance Property

# userInfo

User-provided metadata associated with the attachment.

``` source
var userInfo: [AnyHashable : Any]? { get set }
```

## Discussion

Assign a custom dictionary to this property to store attachment-specific metadata along with the attachment.

Note

The contents of the userInfo dictionary are not represented in Xcode test reports.

## See Also

### Attachment Metadata

var name: String?

The attachment’s name, or `nil` if the attachment is unnamed.

var uniformTypeIdentifier: String

The Uniform Type Identifier (UTI) of the data represented by the attachment.

