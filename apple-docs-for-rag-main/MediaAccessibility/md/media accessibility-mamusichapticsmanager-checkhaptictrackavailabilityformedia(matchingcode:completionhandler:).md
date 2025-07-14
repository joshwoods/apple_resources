

- Media Accessibility
- MAMusicHapticsManager
-  checkHapticTrackAvailabilityForMedia(matchingCode:completionHandler:) 

Instance Method

# checkHapticTrackAvailabilityForMedia(matchingCode:completionHandler:)

Checks whether a haptic track is available for the song with the specified International Standard Recording Code (ISRC).

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func checkHapticTrackAvailabilityForMedia(
    matchingCode internationalStandardRecordingCode: String,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
func isHapticTrackAvailable(forMediaMatching internationalStandardRecordingCode: String) async -> Bool
```

