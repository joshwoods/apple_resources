

- WatchKit
- WKInterfaceController
-  dismissAudioRecorderController() 

Instance Method

# dismissAudioRecorderController()

Dismisses the audio recording interface controller.

watchOS 2.0+

``` source
@MainActor
func dismissAudioRecorderController()
```

## Discussion

Use this method to interrupt media playback and dismiss a modal media interface controller. When you dismiss the recording interface programmatically, the recording controller passes a value of false for the `didSave` parameter of your completion block.

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

Audio Recording Options

Options to specify when recording audio.

