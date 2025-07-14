

- CloudKit
- CKContainer
-  accept(\_:completionHandler:) 

Instance Method

# accept(\_:completionHandler:)

Accepts the specified share metadata.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func accept(
    _ metadata: CKShare.Metadata,
    completionHandler: @escaping (CKShare?, (any Error)?) -> Void
)
```

``` source
func accept(_ metadata: CKShare.Metadata) async throws -> CKShare
```

## Parameters 

`metadata`  

The metadata of the share to accept.

`completionHandler`  

The handler to execute when the process finishes.

## Discussion

The closure doesn’t return a value and takes the following parameters:

- The correspinding share, or `nil` if CloudKit can’t accept the metadata.

- An error if a problem occurs, or `nil` if CloudKit successfully accepts the metadata.

## See Also

### Accessing Container Metadata

func fetchShareMetadata(with: URL, completionHandler: (CKShare.Metadata?, (any Error)?) -> Void)

Fetches the share metadata for the specified share URL.

static let CKAccountChanged: NSNotification.Name

A notification that a container posts when the status of an iCloud account changes.

