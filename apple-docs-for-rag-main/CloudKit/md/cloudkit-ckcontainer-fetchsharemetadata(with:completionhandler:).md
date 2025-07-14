

- CloudKit
- CKContainer
-  fetchShareMetadata(with:completionHandler:) 

Instance Method

# fetchShareMetadata(with:completionHandler:)

Fetches the share metadata for the specified share URL.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func fetchShareMetadata(
    with url: URL,
    completionHandler: @escaping (CKShare.Metadata?, (any Error)?) -> Void
)
```

``` source
func shareMetadata(for url: URL) async throws -> CKShare.Metadata
```

## Parameters 

`url`  

The share URL that CloudKit uses to locate the metadata.

`completionHandler`  

The handler to execute with the fetch results.

## Discussion

The closure doesn’t return a value and takes the following parameters:

- The share metadata, or `nil` if CloudKit can’t find the metadata.

- An error if a problem occurs, or `nil` if CloudKit successfully retrieves the metadata.

## See Also

### Accessing Container Metadata

func accept(CKShare.Metadata, completionHandler: (CKShare?, (any Error)?) -> Void)

Accepts the specified share metadata.

static let CKAccountChanged: NSNotification.Name

A notification that a container posts when the status of an iCloud account changes.

