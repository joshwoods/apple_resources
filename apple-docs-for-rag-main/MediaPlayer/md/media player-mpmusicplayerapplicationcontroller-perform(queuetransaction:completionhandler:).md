

- Media Player
- MPMusicPlayerApplicationController
-  perform(queueTransaction:completionHandler:) 

Instance Method

# perform(queueTransaction:completionHandler:)

Changes the contents of the media items in the queue.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func perform(
    queueTransaction: @escaping (MPMusicPlayerControllerMutableQueue) -> Void,
    completionHandler: @escaping (MPMusicPlayerControllerQueue, (any Error)?) -> Void
)
```

``` source
func perform(queueTransaction: @escaping (MPMusicPlayerControllerMutableQueue) -> Void) async throws -> MPMusicPlayerControllerQueue
```

## Parameters 

`queueTransaction`  

A block that the system calls while it creates the queue.

queue  
The queue to modify.

`completionHandler`  

A block that the system calls after the user accepts the new queue.

queue  
The newly modified queue that the user accepted.

error  
If an error occurred, this parameter holds the error object that explains the error. Otherwise, the value of this parameter is nil.

## Discussion

Perform all of your queue modifications inside of the queue transition block. After the system modifies the queue inside of the queue transition block, it returns the new queue from the completion handler after the user accepts the new queue. Don’t access the completion handler’s queue outside of the completion handler.

If you modify the queue outside of the completion handler, register for the MPMusicPlayerControllerQueueDidChangeNotification notification and ensure your app responds accordingly.

## See Also

### Changing the queue contents

static let MPMusicPlayerControllerQueueDidChange: NSNotification.Name

Indicates the music player’s queue changed.

