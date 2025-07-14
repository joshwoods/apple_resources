

- HealthKit
-  HKAttachment 

Class

# HKAttachment

A file that is attached to a sample in the HealthKit store.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class HKAttachment
```

## Overview

To access the attachment’s data, get a data reader from the attachment store for each attachment.

```
let attachmentStore = HKAttachmentStore(healthStore: store)

let attachments: [HKAttachment]
do {
    attachments = try await attachmentStore.attachments(for: prescription)
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while accessing the attachments for a prescription: \(error.localizedDescription) ***")
}

// Use the attachments here.
print("*** \(attachments.count) attachments found ***")

for attachment in attachments {

    // Get a data reader for the attachment.
    let dataReader = attachmentStore.dataReader(for:   attachment)

    // Read the data here.
}
```

You can then asynchronously access the whole data object.

```
let data: Data
do {
    data = try await dataReader.data
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while accessing the attachment's data. \(error.localizedDescription) ***")
}
```

Alternatively, you can access the file’s contents as an asynchronous sequence of bytes.

```
// Asynchronously access the attachment's bytes.
var data = Data()
do {
    for try await byte in dataReader.bytes {
        // Use the bytes here.
        data.append(byte)
    }
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while reading the attachment's data: \(error.localizedDescription) ***")
}
```

Note

You can only add attachments to HKVisionPrescription, HKGlassesPrescription, and HKContactsPrescription samples. You can also read attachments from clinicalNoteRecord samples.

## Topics

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

var metadata: [String : Any]?

Additional data associated with the attachment in the HealthKit store.

struct AsyncBytes

An asynchronous sequence that returns the attached file as a series of bytes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Related Documentation

class HKVisionPrescription

A sample that stores a vision prescription.

class HKGlassesPrescription

A sample that stores a prescription for glasses.

class HKContactsPrescription

A sample that store a prescription for contacts.

### Attachments

class HKAttachmentStore

The access point for attachments associated with samples in the HealthKit store.

class HKAttachmentDataReader

A reader that provides access to an attachment’s data.

