

- Media Accessibility
- MAMusicHapticsManager
-  removeStatusObserver(\_:) 

Instance Method

# removeStatusObserver(\_:)

Removes the observer monitoring the status of haptic playback for the Now Playing song.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func removeStatusObserver(_ registrationToken: any NSCopying)
```

## See Also

### Observing haptic playback

func addStatusObserver((String, Bool) -> Void) -> (any NSCopying)?

Adds an observer to monitor the status of haptic playback for the Now Playing song.

