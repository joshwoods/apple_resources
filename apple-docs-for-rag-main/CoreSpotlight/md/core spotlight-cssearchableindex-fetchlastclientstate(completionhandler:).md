

- Core Spotlight
- CSSearchableIndex
-  fetchLastClientState(completionHandler:) 

Instance Method

# fetchLastClientState(completionHandler:)

Fetches the app’s most recent client state information asynchronously.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func fetchLastClientState(completionHandler: @escaping (Data?, (any Error)?) -> Void)
```

``` source
func fetchLastClientState() async throws -> Data
```

## Parameters 

`completionHandler`  

The block to call when the request has been *journaled* by the index, which means that the index makes a note that it has to perform this operation. Note that the request may not have completed.

The block receives the following parameter:

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Mentioned in 

Adding your app’s content to Spotlight indexes

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func fetchLastClientState() async throws -> Data
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Batching index updates

func beginBatch()

Begins a batch of updates to an index.

func endBatch(withClientState: Data, completionHandler: (((any Error)?) -> Void)?)

Ends a batch of index updates and stores the specified state information.

func endIndexBatch(expectedClientState: Data?, newClientState: Data, completionHandler: (((any Error)?) -> Void)?)

Ends a batch of index updates and stores the specified state information.

