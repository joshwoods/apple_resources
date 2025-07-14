

- HealthKit
- HKAttachmentDataReader
-  bytes 

Instance Property

# bytes

An asynchronous sequence that provides the attachment’s data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
var bytes: HKAttachment.AsyncBytes { get }
```

## Discussion

Use this property to access the file’s contents as an asynchronous sequence of bytes.

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

## See Also

### Reading attachment data

var data: Data

The abstract’s data.

var progress: Progress

An object you can use to track the progress while reading an attachment’s data.

