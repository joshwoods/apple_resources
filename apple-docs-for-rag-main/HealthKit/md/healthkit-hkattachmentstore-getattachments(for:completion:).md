

- HealthKit
- HKAttachmentStore
-  getAttachments(for:completion:) 

Instance Method

# getAttachments(for:completion:)

Returns all the attachments for the specified object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
func getAttachments(
    for object: HKObject,
    completion: @escaping ([HKAttachment]?, (any Error)?) -> Void
)
```

``` source
func attachments(for object: HKObject) async throws -> [HKAttachment]
```

## Parameters 

`object`  

An object from the HealthKit store.

`completion`  

A completion handler that the system calls to return the attachment. This handler takes the following parameters:

attachments  
An array of attachments. If an error occurs, the system sets this parameter to `nil`.

error  
If an error occurred, this parameter contains information about the error. Otherwise, it’s `nil`.

## Discussion

Call this method to get all the attachments for the specified object.

```
let attachments: [HKAttachment]
do {
    attachments = try await attachmentStore.attachments(for: prescription)
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while accessing the attachments for a prescription: \(error.localizedDescription) ***")
}

// Use the attachments here.
```

## See Also

### Accessing attachments

func dataReader(for: HKAttachment) -> HKAttachmentDataReader

Returns a data reader for the attachment.

func getData(for: HKAttachment, completion: (Data?, (any Error)?) -> Void) -> Progress

Returns an attachment’s data.

func streamData(for: HKAttachment, dataHandler: (Data?, (any Error)?, Bool) -> Void) -> Progress

Asynchronously returns the attachment’s data.

