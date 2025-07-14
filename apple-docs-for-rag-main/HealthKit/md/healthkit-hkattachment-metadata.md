

- HealthKit
- HKAttachment
-  metadata 

Instance Property

# metadata

Additional data associated with the attachment in the HealthKit store.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var metadata: [String : Any]? { get }
```

## Discussion

The metadata dictionary contains extra information describing this object. The dictionary’s keys are all strings. The values can be strings, numbers, or dates. For a complete list of predefined metadata keys, see Metadata Keys.

Using predefined keys helps facilitate sharing data between apps; however, you’re also encouraged to create your own, custom keys as needed to extend a HealthKit object’s capabilities.

## See Also

### Accessing attachment data

var name: String

The name of the attached file.

var identifier: UUID

The universally unique identifier for the attached file.

var contentType: UTType

The type of data stored in the attached file.

var size: Int

The attachment’s size (in bytes).

var creationDate: Date

The attachment’s creation date.

struct AsyncBytes

An asynchronous sequence that returns the attached file as a series of bytes.

