

- AppKit
- NSSoundDelegate
-  sound(\_:didFinishPlaying:) 

Instance Method

# sound(\_:didFinishPlaying:)

This delegate method is called when an `NSSound` instance has completed playback of its sound data.

macOS

``` source
@MainActor
optional func sound(
    _ sound: NSSound,
    didFinishPlaying flag: Bool
)
```

## Parameters 

`sound`  

The `NSSound` that has completed playback of its sound data.

`flag`  

true when playback was successful; false otherwise.

## See Also

### Related Documentation

Sound Programming Topics for Cocoa

