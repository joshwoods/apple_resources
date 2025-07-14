

- AVFoundation
- AVPlayerItem
-  canPlayFastForward 

Instance Property

# canPlayFastForward

A Boolean value that indicates whether the item can be fast forwarded.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var canPlayFastForward: Bool { get }
```

## Discussion

An item can be fast forwarded if its rate can be greater than `1.0`.

## See Also

### Determining Playback Capabilities

var canPlayReverse: Bool

A Boolean value that indicates whether the item can play in reverse.

var canPlayFastReverse: Bool

A Boolean value that indicates whether the item can be quickly reversed.

var canPlaySlowForward: Bool

A Boolean value that indicates whether the item can play slower than normal.

var canPlaySlowReverse: Bool

A Boolean value that indicates whether the item can play slowly backward.

