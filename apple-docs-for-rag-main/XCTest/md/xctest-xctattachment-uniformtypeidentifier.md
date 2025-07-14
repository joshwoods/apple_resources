

- XCTest
- XCTAttachment
-  uniformTypeIdentifier 

Instance Property

# uniformTypeIdentifier

The Uniform Type Identifier (UTI) of the data represented by the attachment.

``` source
var uniformTypeIdentifier: String { get }
```

## Mentioned in 

Adding Attachments to Tests, Activities, and Issues

## Discussion

Uniform Type Identifiers (UTIs) are Apple-defined identifiers that uniquely identify a particular type of data, such as a JPEG image or text document. Every XCTAttachment instance stores a UTI string that indicates the type of data represented by the attachment.

When you create an attachment with an XCTAttachment convenience initializer such as init(contentsOfFileAtURL:) or init(plistObject:), XCTest determines an appropriate UTI to use for the provided data. See each convenience initializer for more information about the UTIs it uses.

Where possible, you should use the XCTAttachment convenience initializers to create attachments for known data types. If you need to create an attachment with a manually specified UTI (such as for a custom data format used by your app), use one of the following initializers instead:

- init(archivableObject:uniformTypeIdentifier:) for custom data stored in an object that conforms to NSSecureCoding

- init(contentsOfFileAtURL:uniformTypeIdentifier:) for reading the contents of a file with a known custom UTI

- init(data:uniformTypeIdentifier:) for data stored in memory with a known custom UTI

- init(uniformTypeIdentifier:name:payload:userInfo:) for a data payload with a custom UTI, name, and user info dictionary

For more information about UTIs, see Uniform Type Identifiers Overview. For a list of system-declared UTIs, see Uniform Type Identifiers Reference.

## See Also

### Attachment Metadata

var name: String?

The attachment’s name, or `nil` if the attachment is unnamed.

var userInfo: [AnyHashable : Any]?

User-provided metadata associated with the attachment.

