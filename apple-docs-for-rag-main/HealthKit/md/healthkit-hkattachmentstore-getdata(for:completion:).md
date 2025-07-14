

- HealthKit
- HKAttachmentStore
-  getData(for:completion:) 

Instance Method

# getData(for:completion:)

Returns an attachment’s data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
func getData(
    for attachment: HKAttachment,
    completion: @escaping (Data?, (any Error)?) -> Void
) -> Progress
```

## Parameters 

`attachment`  

An attachment associated with an object in the HealthKit store.

`completion`  

A completion handler that the system calls to return the data. This handler takes the following parameters:

attachmentData  
A Data object that contains the attachment’s contents. If an error occurs, the system sets this parameter to `nil`.

error  
If an error occurred, this parameter contains information about the error. Otherwise, it’s `nil`.

## Discussion

Call this method to read the attachment’s contents directly from the attachment store.

```
let progress = attachmentStore.getData(for: myAttachment) { data, error in
    if let error {
        // Handle the error here.
        fatalError("*** An error occurred while accessing the attachment's data. \(error.localizedDescription) ***")
    }

    // Use the data here.
}

// Monitor the progress here.
```

## See Also

### Accessing attachments

func getAttachments(for: HKObject, completion: ([HKAttachment]?, (any Error)?) -> Void)

Returns all the attachments for the specified object.

func dataReader(for: HKAttachment) -> HKAttachmentDataReader

Returns a data reader for the attachment.

func streamData(for: HKAttachment, dataHandler: (Data?, (any Error)?, Bool) -> Void) -> Progress

Asynchronously returns the attachment’s data.

