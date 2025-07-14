

- AVFAudio
- AVAudioApplication
-  setInputMuted(\_:) 

Instance Method

# setInputMuted(\_:)

Sets a Boolean value that indicates whether the app’s audio input is in a muted state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func setInputMuted(_ muted: Bool) throws
```

## Parameters 

`muted`  

A Boolean value that indicates the new mute state.

## Discussion

In platforms that use AVAudioSession, setting the value to true mutes all sources of audio input in the app. In macOS, the system instead invokes the callback that you register by calling setInputMuteStateChangeHandler(_:) to handle input muting.

Note

This setting is specific to your app and doesn’t affect hardware mute state.

## See Also

### Managing audio input mute state

var isInputMuted: Bool

A Boolean value that indicates whether the app’s audio input is in a muted state.

class let inputMuteStateChangeNotification: NSNotification.Name

A notification the system posts when the app’s audio input mute state changes.

func setInputMuteStateChangeHandler(((Bool) -> Bool)?) throws

Sets a callback to handle changes to application-level audio muting states.

