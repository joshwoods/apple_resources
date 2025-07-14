

- HealthKit
- HKAttachmentStore
-  streamData(for:dataHandler:) 

Instance Method

# streamData(for:dataHandler:)

Asynchronously returns the attachment’s data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
func streamData(
    for attachment: HKAttachment,
    dataHandler: @escaping (Data?, (any Error)?, Bool) -> Void
) -> Progress
```

## Parameters 

`attachment`  

An attachment associated with an object in the HealthKit store.

`dataHandler`  

A closure that the system calls repeatedly to return the attachment’s contents. This closure takes the following parameters:

dataChunk  
A data object that contains the next chunk of the attachment’s contents. If an error occurred, the system sets this property to `nil`.

error  
If an error occurred, this parameter contains information about the error. Otherwise, it’s `nil`.

done  
A Boolean value that indicates whether the transfer is complete. If this is the last `dataChunk`, the system sets this property to true.

## Discussion

Call this method to incrementally read the attachment’s contents directly from the attachment store.

```
var data = Data()
attachmentStore.streamData(for: myAttachment) { dataChunk, error, done in

    if let error {
        // Handle the error here.
        fatalError("*** An error occurred while streaming the attachment's data. \(error.localizedDescription) ***")
    }

    guard let dataChunk else { return }

    data.append(dataChunk)

    if done {
        // Use the attachment's data here.
        print(data)
    }
}
```

## See Also

### Accessing attachments

func getAttachments(for: HKObject, completion: ([HKAttachment]?, (any Error)?) -> Void)

Returns all the attachments for the specified object.

func dataReader(for: HKAttachment) -> HKAttachmentDataReader

Returns a data reader for the attachment.

func getData(for: HKAttachment, completion: (Data?, (any Error)?) -> Void) -> Progress

Returns an attachment’s data.

