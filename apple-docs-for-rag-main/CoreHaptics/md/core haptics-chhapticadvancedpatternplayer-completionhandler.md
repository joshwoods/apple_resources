

- Core Haptics
- CHHapticAdvancedPatternPlayer
-  completionHandler 

Instance Property

# completionHandler

A completion block that runs after the haptic finishes playing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var completionHandler: CHHapticAdvancedPatternPlayerCompletionHandler { get set }
```

**Required**

## See Also

### Setting Playback Properties

var loopEnabled: Bool

A Boolean that determines whether the haptic repeats itself on completion.

**Required**

var loopEnd: TimeInterval

The time at which to end looping haptic playback.

**Required**

var playbackRate: Float

The playback rate of the haptic player.

**Required**

typealias CHHapticAdvancedPatternPlayerCompletionHandler

A typealias for the completion handler to run after a haptic finishes playback.

