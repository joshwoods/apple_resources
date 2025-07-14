

- PHASE
- PHASESoundEvent
-  seek(to:completion:) 

Instance Method

# seek(to:completion:)

Advances the sound event’s playback position to a specific time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func seek(
    to time: Double,
    completion handler: ((PHASESoundEvent.SeekHandlerReason) -> Void)? = nil
)
```

``` source
func seek(to time: Double) async -> PHASESoundEvent.SeekHandlerReason
```

## Parameters 

`time`  

The playback position to advance to. The framework scales this value by unitsPerSecond.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func seek(to time: Double) async -> PHASESoundEvent.SeekHandlerReason
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Seeking a Time

enum SeekHandlerReason

Indicates the status after a sound event changes its playback position.

