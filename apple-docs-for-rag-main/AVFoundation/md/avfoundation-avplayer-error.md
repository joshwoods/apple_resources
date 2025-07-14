

- AVFoundation
- AVPlayer
-  error 

Instance Property

# error

An error that caused a failure.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var error: (any Error)? { get }
```

## Discussion

By default, this value is `nil`. If a player reaches a AVPlayer.Status.failed, the system populates this value with an error that describes the failure.

## See Also

### Determining Player Readiness

var status: AVPlayer.Status

A value that indicates the readiness of a player object for playback.

enum Status

Status values that indicate whether a player can successfully play media.

