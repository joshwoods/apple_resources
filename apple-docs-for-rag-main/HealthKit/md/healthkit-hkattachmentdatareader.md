

- HealthKit
-  HKAttachmentDataReader 

Class

# HKAttachmentDataReader

A reader that provides access to an attachment’s data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
class HKAttachmentDataReader
```

## Overview

To access the attachment’s data, get a data reader from the attachment store.

```
let attachmentStore = HKAttachmentStore(healthStore: store)

// Get a data reader for the attachment.
let dataReader = attachmentStore.dataReader(for: myAttachment)
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

## Topics

### Reading attachment data

var data: Data

The abstract’s data.

var bytes: HKAttachment.AsyncBytes

An asynchronous sequence that provides the attachment’s data.

var progress: Progress

An object you can use to track the progress while reading an attachment’s data.

### Accessing the attachment object

var attachment: HKAttachment

An attachment object that represents the file from which the reader is reading.

## See Also

### Attachments

class HKAttachment

A file that is attached to a sample in the HealthKit store.

class HKAttachmentStore

The access point for attachments associated with samples in the HealthKit store.

