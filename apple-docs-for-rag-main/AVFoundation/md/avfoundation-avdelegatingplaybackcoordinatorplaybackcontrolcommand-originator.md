

- AVFoundation
- AVDelegatingPlaybackCoordinatorPlaybackControlCommand
-  originator 

Instance Property

# originator

The participant that causes the coordinator to issue the command.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var originator: AVCoordinatedPlaybackParticipant? { get }
```

## Discussion

Only commands that the system issues on behalf of another participant contain an originator. Local commands to coordinate rate change, or those that originate from a call to reapplyCurrentItemStateToPlaybackControlDelegate(), don’t.

Note

You can use the existance of an originator value to show a user interface that indicates another partipant’s action.

## See Also

### Accessing Command Details

var expectedCurrentItemIdentifier: String

An item identifier the coordinator issues the command for.

