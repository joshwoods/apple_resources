

- WatchKit
- Storyboard support
- WKInterfaceController
-  Audio Recording Options 

API Collection

# Audio Recording Options

Options to specify when recording audio.

## Topics

### Constants

let WKAudioRecorderControllerOptionsActionTitleKey: String

The title to display on the button that the user taps to accept a recording. The value of this key is an NSString object. If you do not specify this option, the button title is set to “Save”.

let WKAudioRecorderControllerOptionsAlwaysShowActionTitleKey: String

The behavior for showing the action button. The value of this key is an NSNumber object with a Boolean value. When the value is true, the recording interface always shows the action button. When the value is false, the sheet shows the button only after the user has recorded some audio. The default value for this option is YES.

let WKAudioRecorderControllerOptionsAutorecordKey: String

The automatic recording behavior of the action sheet. The value of this key is an NSNumber object with a Boolean value. When the value is true, the recording interface starts recording as soon as it is presented. When the value is false, the user must start recording manually. The default value for this option is true.

let WKAudioRecorderControllerOptionsMaximumDurationKey: String

The maximum length of recorded audio clips. The value of this key is an NSNumber object with an TimeInterval value containing the maximum duration in seconds. If you do not specify this option, there is no maximum recording time.

## See Also

### Presenting video and audio interfaces

func presentMediaPlayerController(with: URL, options: [AnyHashable : Any]?, completion: (Bool, TimeInterval, (any Error)?) -> Void)

Displays a modal interface for playing the specified media file.

Media Player Options

Keys indicating media playback options.

func dismissMediaPlayerController()

Dismisses the media interface controller.

func presentAudioRecorderController(withOutputURL: URL, preset: WKAudioRecorderPreset, options: [AnyHashable : Any]?, completion: (Bool, (any Error)?) -> Void)

Display a standard interface for recording audio from the user’s Apple Watch.

enum WKAudioRecorderPreset

Constants indicating the quality of audio recordings.

func dismissAudioRecorderController()

Dismisses the audio recording interface controller.

