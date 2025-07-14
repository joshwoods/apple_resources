

- AppKit
-  NSSoundDelegate 

Protocol

# NSSoundDelegate

A set of optional methods implemented by delegates of NSSound objects.

macOS

``` source
protocol NSSoundDelegate : NSObjectProtocol
```

## Topics

### Playing Sounds

func sound(NSSound, didFinishPlaying: Bool)

This delegate method is called when an `NSSound` instance has completed playback of its sound data.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Detecting When a Sound Finishes Playing

var delegate: (any NSSoundDelegate)?

The sound’s delegate.

