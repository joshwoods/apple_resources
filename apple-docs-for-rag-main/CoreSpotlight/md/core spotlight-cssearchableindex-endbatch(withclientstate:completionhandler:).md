

- Core Spotlight
- CSSearchableIndex
-  endBatch(withClientState:completionHandler:) 

Instance Method

# endBatch(withClientState:completionHandler:)

Ends a batch of index updates and stores the specified state information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func endBatch(
    withClientState clientState: Data,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func endBatch(withClientState clientState: Data) async throws
```

## Parameters 

`clientState`  

Up to 250 bytes of information that can help you recover from a crash and resume indexing.

`completionHandler`  

The block that’s called after the client state has been stored.

The block receives the following parameter:

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func endBatch(withClientState clientState: Data) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Batching index updates

func beginBatch()

Begins a batch of updates to an index.

func endIndexBatch(expectedClientState: Data?, newClientState: Data, completionHandler: (((any Error)?) -> Void)?)

Ends a batch of index updates and stores the specified state information.

func fetchLastClientState(completionHandler: (Data?, (any Error)?) -> Void)

Fetches the app’s most recent client state information asynchronously.

