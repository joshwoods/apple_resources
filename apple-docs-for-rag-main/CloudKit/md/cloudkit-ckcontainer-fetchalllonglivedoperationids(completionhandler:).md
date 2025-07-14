

- CloudKit
- CKContainer
-  fetchAllLongLivedOperationIDs(completionHandler:) 

Instance Method

# fetchAllLongLivedOperationIDs(completionHandler:)

Fetches the IDs of any long-lived operations that are running.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.12+tvOS 9.2+visionOSwatchOS 3.0+Swift 4.2+

``` source
@preconcurrency
func fetchAllLongLivedOperationIDs(completionHandler: @escaping ([CKOperation.ID]?, (any Error)?) -> Void)
```

## Parameters 

`completionHandler`  

The closure to execute with the fetch results.

## Discussion

The closure doesn’t return a value and takes the following parameters:

- The IDs of all of the long-lived operations that are running.

- An error if a problem occurs, or `nil` if CloudKit successfully retrieves the IDs.

A long-lived operation is one that continues to run after the user closes your app. When a long-lived operation completes, or your app or the system cancels it, it’s no longer active and CloudKit doesn’t include its ID in `outstandingOperationsByIDs`. An operation is complete when the system calls its completion handler.

Use the fetchLongLivedOperationWithID:completionHandler: method to fetch the operation for a specific ID.

## See Also

### Fetching Long-Lived Operations

func fetchLongLivedOperation(withID: CKOperation.ID, completionHandler: (CKOperation?, (any Error)?) -> Void)

Fetches the long-lived operation for the specified operation ID.

