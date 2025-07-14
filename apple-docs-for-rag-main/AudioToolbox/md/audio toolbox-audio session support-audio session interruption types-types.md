

- Audio Toolbox
- Audio Session Support
-  Audio Session Interruption Types 

API Collection

# Audio Session Interruption Types

## Topics

### Constants

var kAudioSessionInterruptionType_ShouldNotResume: Int

Indicates that the interruption that has just ended was one for which it is not appropriate to resume playback; for example, your app had been interrupted by iPod playback.

var kAudioSessionInterruptionType_ShouldResume: Int

Indicates that the interruption that has just ended was one for which it is appropriate to immediately resume playback; for example, an incoming phone call was rejected by the user.

Deprecated

