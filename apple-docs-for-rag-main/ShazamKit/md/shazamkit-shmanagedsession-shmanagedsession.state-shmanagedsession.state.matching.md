

- ShazamKit
- SHManagedSession
- SHManagedSession.State
-  SHManagedSession.State.matching 

Case

# SHManagedSession.State.matching

The session is recording and making at least one match attempt.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case matching
```

## Discussion

When a session is in this state, the framework ignores calls to prepare().

## See Also

### Getting session states

case idle

The session isn’t recording or making a match attempt.

case prerecording

The session has the resources it needs for matching and is prerecording.

