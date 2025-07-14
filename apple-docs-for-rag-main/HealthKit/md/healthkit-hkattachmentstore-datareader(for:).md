

- HealthKit
- HKAttachmentStore
-  dataReader(for:) 

Instance Method

# dataReader(for:)

Returns a data reader for the attachment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
func dataReader(for attachment: HKAttachment) -> HKAttachmentDataReader
```

## Parameters 

`attachment`  

An attachment associated with an object in the HealthKit store.

## Discussion

Call this method to access a data reader for the attachment’s contents.

```
// Get a data reader for the attachment.
let dataReader = attachmentStore.dataReader(for: myAttachment)
```

You can then read the attachment’s contents from the data reader.

```
let data: Data
do {
    data = try await dataReader.data
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while accessing the attachment's data. \(error.localizedDescription) ***")
}

// Use the data here.
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

## See Also

### Accessing attachments

func getAttachments(for: HKObject, completion: ([HKAttachment]?, (any Error)?) -> Void)

Returns all the attachments for the specified object.

func getData(for: HKAttachment, completion: (Data?, (any Error)?) -> Void) -> Progress

Returns an attachment’s data.

func streamData(for: HKAttachment, dataHandler: (Data?, (any Error)?, Bool) -> Void) -> Progress

Asynchronously returns the attachment’s data.

