

- HealthKit
- HKAttachment
-  name 

Instance Property

# name

The name of the attached file.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var name: String { get }
```

## See Also

### Accessing attachment data

var identifier: UUID

The universally unique identifier for the attached file.

var contentType: UTType

The type of data stored in the attached file.

var size: Int

The attachment’s size (in bytes).

var creationDate: Date

The attachment’s creation date.

var metadata: [String : Any]?

Additional data associated with the attachment in the HealthKit store.

struct AsyncBytes

An asynchronous sequence that returns the attached file as a series of bytes.

