

- Media Accessibility
- MAMusicHapticsManager
-  addStatusObserver(\_:) 

Instance Method

# addStatusObserver(\_:)

Adds an observer to monitor the status of haptic playback for the Now Playing song.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func addStatusObserver(_ statusHandler: @escaping (String, Bool) -> Void) -> (any NSCopying)?
```

## See Also

### Observing haptic playback

func removeStatusObserver(any NSCopying)

Removes the observer monitoring the status of haptic playback for the Now Playing song.

