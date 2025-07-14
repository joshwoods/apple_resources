

- XCTest
- XCTAttachment
-  XCTAttachment.Lifetime 

Enumeration

# XCTAttachment.Lifetime

The possible lifetime values for a test attachment.

``` source
enum Lifetime
```

## Topics

### Attachment Lifetimes

case deleteOnSuccess

Indicates that the attachment should be deleted if the test passes.

case keepAlways

Indicates that the attachment should be persisted as part of the test’s results even if the test passes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting an Attachment’s Lifetime

var lifetime: XCTAttachment.Lifetime

Indicates whether the attachment is kept or discarded when its associated test passes.

