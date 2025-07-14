

- AVFoundation
- AVPlayerItem
-  error 

Instance Property

# error

The error that caused the player item to fail.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var error: (any Error)? { get }
```

## Discussion

The value of this property is an error that describes what caused the player item to no longer be able to be played.

If the receiver’s status is not AVPlayerItem.Status.failed, the value of this property is `nil`.

## See Also

### Determining Readiness

var status: AVPlayerItem.Status

The status of the player item.

enum Status

The statuses for a player item.

