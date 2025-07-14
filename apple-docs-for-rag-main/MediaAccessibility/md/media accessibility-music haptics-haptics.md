

- Media Accessibility
-  Music Haptics 

API Collection

# Music Haptics

Play haptic tracks along with known music tracks.

## Overview

Music Haptics is an accessibility feature that allows a person to indicate that they want to play haptic tracks along with known music tracks. This feature allows people who are deaf or hard of hearing to enjoy music through tactile feedback. A person can turn on this feature in Settings \> Accessibility \> Music Haptics. If you play music in your app, you can support haptic feedback for known songs.

### Support Music Haptics

To support Music Haptics in your app:

- Add the MusicHapticsSupported key to your app’s `Info.plist` and set its value to `YES`.

- Check whether Music Haptics is on using isActive on the shared instance of MAMusicHapticsManager.

- Register for the activeStatusDidChangeNotification notification to listen for changes in the Music Haptics setting.

- Supply a known song’s International Standard Recording Code (ISRC) as part of the nowPlayingInfo dictionary of MPNowPlayingInfoCenter, using the key MPNowPlayingInfoPropertyInternationalStandardRecordingCode. For more information about becoming the Now Playing app, refer to Becoming a now playable app.

### Indicate haptic playback status

To indicate the status of haptic playback for Music Haptics, you can use the following symbols:

| Symbol name | Status | API |
|----|----|----|
| `"apple.haptics.and.music.note"` | Active | isActive is `true` |
| `"apple.haptics.and.music.note.slash"` | Paused | isActive is `false` |
| `"apple.haptics.and.exclamationmark.triangle"` | Unavailable | checkHapticTrackAvailabilityForMedia(matchingCode:completionHandler:) is `false` |

For more details about using these symbols, refer to the SF Symbols app.

## Topics

### Music Haptics

class MAMusicHapticsManager

A class that reports information about the Music Haptics feature.

## See Also

### Features

Captions

Coordinate the presentation of closed-captioned data for your app’s media files.

Flashing lights

Detect, mitigate, and inform people about flashing lights in media content.

