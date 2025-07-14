

- CloudKit
- CKContainer
-  fetchLongLivedOperation(withID:completionHandler:) 

Instance Method

# fetchLongLivedOperation(withID:completionHandler:)

Fetches the long-lived operation for the specified operation ID.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.12+tvOS 9.2+visionOSwatchOS 3.0+Swift 4.2+

``` source
@preconcurrency
func fetchLongLivedOperation(
    withID operationID: CKOperation.ID,
    completionHandler: @escaping (CKOperation?, (any Error)?) -> Void
)
```

## Parameters 

`operationID`  

The operation’s ID.

`completionHandler`  

The closure to execute with the fetch results.

## Discussion

The closure doesn’t return a value and takes the following parameters:

- The long-lived operation. If the operation completes, or your app or the system cancels it, this parameter is `nil`.

- An error if a problem occurs, or `nil` if CloudKit successfully retrieves the operation.

A long-lived operation is one that continues to run after the user closes your app. When a long-lived operation completes, the system calls its completion block to notify you.

## See Also

### Fetching Long-Lived Operations

func fetchAllLongLivedOperationIDs(completionHandler: ([CKOperation.ID]?, (any Error)?) -> Void)

Fetches the IDs of any long-lived operations that are running.

