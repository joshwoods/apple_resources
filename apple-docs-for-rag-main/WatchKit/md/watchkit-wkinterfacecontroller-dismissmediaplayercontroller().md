

- WatchKit
- WKInterfaceController
-  dismissMediaPlayerController() 

Instance Method

# dismissMediaPlayerController()

Dismisses the media interface controller.

watchOS 2.0+

``` source
@MainActor
func dismissMediaPlayerController()
```

## Discussion

Use this method to dismiss a modal media interface controller programmatically. When you dismiss the media interface programmatically, WatchKit passes a value of false for the `didPlayToEnd` parameter of your completion block and passes a value of `0.0` for the`endTime` parameter.

## See Also

### Presenting video and audio interfaces

func presentMediaPlayerController(with: URL, options: [AnyHashable : Any]?, completion: (Bool, TimeInterval, (any Error)?) -> Void)

Displays a modal interface for playing the specified media file.

Media Player Options

Keys indicating media playback options.

func presentAudioRecorderController(withOutputURL: URL, preset: WKAudioRecorderPreset, options: [AnyHashable : Any]?, completion: (Bool, (any Error)?) -> Void)

Display a standard interface for recording audio from the user’s Apple Watch.

enum WKAudioRecorderPreset

Constants indicating the quality of audio recordings.

Audio Recording Options

Options to specify when recording audio.

func dismissAudioRecorderController()

Dismisses the audio recording interface controller.

