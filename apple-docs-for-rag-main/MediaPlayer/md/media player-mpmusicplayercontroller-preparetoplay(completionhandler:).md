

- Media Player
- MPMusicPlayerController
-  prepareToPlay(completionHandler:) 

Instance Method

# prepareToPlay(completionHandler:)

Prepares a music player for playback.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func prepareToPlay(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func prepareToPlay() async throws
```

## Parameters 

`completionHandler`  

A block that the system call after it buffers the first item in the queue and it’s ready to play.

error  
If an error occurred, this parameter holds the error object that explains the error. Otherwise, the value of this parameter is nil.

## Discussion

Call this function to ensure that the system buffers the first item in the queue and it’s ready to play. The system executes the code in the completion handler after it buffers the first item in the queue.

