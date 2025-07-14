

- AVFAudio
- AVAudioApplication
-  isInputMuted 

Instance Property

# isInputMuted

A Boolean value that indicates whether the app’s audio input is in a muted state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var isInputMuted: Bool { get }
```

## Discussion

Set a new value for this property by calling the setInputMuted(_:) method.

## See Also

### Managing audio input mute state

func setInputMuted(Bool) throws

Sets a Boolean value that indicates whether the app’s audio input is in a muted state.

class let inputMuteStateChangeNotification: NSNotification.Name

A notification the system posts when the app’s audio input mute state changes.

func setInputMuteStateChangeHandler(((Bool) -> Bool)?) throws

Sets a callback to handle changes to application-level audio muting states.

