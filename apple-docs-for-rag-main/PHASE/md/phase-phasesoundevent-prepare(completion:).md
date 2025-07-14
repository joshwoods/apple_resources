

- PHASE
- PHASESoundEvent
-  prepare(completion:) 

Instance Method

# prepare(completion:)

Enables a sound event to play and runs the argument code when the sound event plays back.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func prepare(completion handler: ((PHASESoundEvent.PrepareHandlerReason) -> Void)? = nil)
```

``` source
func prepare() async -> PHASESoundEvent.PrepareHandlerReason
```

## Parameters 

`handler`  

Code the framework runs when sound event preparation completes. If you pass `nil`, no code runs when preparation completes.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func prepare() async -> PHASESoundEvent.PrepareHandlerReason
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This function instructs the engine to prepare a sound event and returns immediately. When the preparation completes or fails, the framework runs `completionHandler`.

If you call start(completion:) before `completionHandler` runs, the framework queues the sound event to occur when preparation completes.

## See Also

### Preparing Playback

enum PrepareHandlerReason

Indicates the results of sound-event preparation.

var prepareState: PHASESoundEvent.PrepareState

The status of sound-event preparation.

enum PrepareState

Indicates the state of sound-event preparation.

