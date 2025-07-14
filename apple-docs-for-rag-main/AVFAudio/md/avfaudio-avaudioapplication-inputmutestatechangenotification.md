

- AVFAudio
- AVAudioApplication
-  inputMuteStateChangeNotification 

Type Property

# inputMuteStateChangeNotification

A notification the system posts when the app’s audio input mute state changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class let inputMuteStateChangeNotification: NSNotification.Name
```

## Topics

### User information keys

class let muteStateKey: String

A user information key to determine the app’s audio mute state.

## See Also

### Managing audio input mute state

var isInputMuted: Bool

A Boolean value that indicates whether the app’s audio input is in a muted state.

func setInputMuted(Bool) throws

Sets a Boolean value that indicates whether the app’s audio input is in a muted state.

func setInputMuteStateChangeHandler(((Bool) -> Bool)?) throws

Sets a callback to handle changes to application-level audio muting states.

