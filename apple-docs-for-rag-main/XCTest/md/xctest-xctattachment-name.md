

- XCTest
- XCTAttachment
-  name 

Instance Property

# name

The attachment’s name, or `nil` if the attachment is unnamed.

``` source
var name: String? { get set }
```

## Discussion

Set an attachment’s name property to a custom string to provide a descriptive name for the attachment within Xcode’s test reports.

## See Also

### Attachment Metadata

var uniformTypeIdentifier: String

The Uniform Type Identifier (UTI) of the data represented by the attachment.

var userInfo: [AnyHashable : Any]?

User-provided metadata associated with the attachment.

