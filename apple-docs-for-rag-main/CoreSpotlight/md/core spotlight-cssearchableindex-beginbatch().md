

- Core Spotlight
- CSSearchableIndex
-  beginBatch() 

Instance Method

# beginBatch()

Begins a batch of updates to an index.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func beginBatch()
```

## Discussion

Don’t call this method again before endBatch(withClientState:completionHandler:) has returned. (You can call it again before the completion handler passed to endBatch(withClientState:completionHandler:) has been called.)

## See Also

### Batching index updates

func endBatch(withClientState: Data, completionHandler: (((any Error)?) -> Void)?)

Ends a batch of index updates and stores the specified state information.

func endIndexBatch(expectedClientState: Data?, newClientState: Data, completionHandler: (((any Error)?) -> Void)?)

Ends a batch of index updates and stores the specified state information.

func fetchLastClientState(completionHandler: (Data?, (any Error)?) -> Void)

Fetches the app’s most recent client state information asynchronously.

