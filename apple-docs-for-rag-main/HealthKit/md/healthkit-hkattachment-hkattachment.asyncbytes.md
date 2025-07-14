

- HealthKit
- HKAttachment
-  HKAttachment.AsyncBytes 

Structure

# HKAttachment.AsyncBytes

An asynchronous sequence that returns the attached file as a series of bytes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
struct AsyncBytes
```

## Overview

To access the attachment file as an asynchronous sequence of bytes, get a data reader from the attachment store, and then access its bytes using a `for-await-in` loop.

```
// Get a data reader for the attachment.
let dataReader = attachmentStore.dataReader(for: myAttachment)

// Asynchronously access the attachment's bytes.
var data = Data()
do {
    for try await byte in dataReader.bytes {
        data.append(byte)
    }
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while reading the attachment's data: \(error.localizedDescription) ***")
}

// Use the data here.
```

## Relationships

### Conforms To

- AsyncSequence

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

var metadata: [String : Any]?

Additional data associated with the attachment in the HealthKit store.

