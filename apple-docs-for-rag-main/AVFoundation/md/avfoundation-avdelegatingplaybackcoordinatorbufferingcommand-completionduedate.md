

- AVFoundation
- AVDelegatingPlaybackCoordinatorBufferingCommand
-  completionDueDate 

Instance Property

# completionDueDate

The deadline by which the coordinator expects the delegate to complete execution of a command.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var completionDueDate: Date? { get }
```

## Discussion

A command that expects buffering in preparation for playback requires that the delegate call the command’s completion handler by the deadline. The delegate needs to complete the command by this date to keep up with the group. Alternatively, have the delegate begin a stall recovery suspension, and communicate that state to the other participants.

Completing the command after this date means that the coordinator likely sends a play command that isn’t for the current state.

## See Also

### Accessing Command Details

var anticipatedPlaybackRate: Float

The rate at which the coordinator expects the current item to play.

