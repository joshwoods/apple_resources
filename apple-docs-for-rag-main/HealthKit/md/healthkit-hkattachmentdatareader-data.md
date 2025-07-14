

- HealthKit
- HKAttachmentDataReader
-  data 

Instance Property

# data

The abstract’s data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
var data: Data { get async throws }
```

## Discussion

Use this property to asynchronously access the attachment’s data as a single data object.

```
let data: Data
do {
    data = try await dataReader.data
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while accessing the attachment's data. \(error.localizedDescription) ***")
}
```

## See Also

### Reading attachment data

var bytes: HKAttachment.AsyncBytes

An asynchronous sequence that provides the attachment’s data.

var progress: Progress

An object you can use to track the progress while reading an attachment’s data.

