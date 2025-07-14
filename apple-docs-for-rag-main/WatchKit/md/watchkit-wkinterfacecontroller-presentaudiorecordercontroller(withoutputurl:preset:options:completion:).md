

- WatchKit
- WKInterfaceController
-  presentAudioRecorderController(withOutputURL:preset:options:completion:) 

Instance Method

# presentAudioRecorderController(withOutputURL:preset:options:completion:)

Display a standard interface for recording audio from the user’s Apple Watch.

watchOS 2.0+

``` source
@MainActor
func presentAudioRecorderController(
    withOutputURL URL: URL,
    preset: WKAudioRecorderPreset,
    options: [AnyHashable : Any]? = nil,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
@MainActor
func presentAudioRecorderController(
    withOutputURL URL: URL,
    preset: WKAudioRecorderPreset,
    options: [AnyHashable : Any]? = nil
) async throws -> Bool
```

## Parameters 

`URL`  

The URL at which to store the recorded output. The filename extension determines the type of audio to record. You may specify the extensions `.wav`, `.mp4`, and `.m4a`.

`preset`  

The recording quality. Specify the constant that best represents the type of audio you want to record. For a list of possible values, see WKAudioRecorderPreset.

`options`  

A dictionary of options to use during recording. If you specify `nil` for this parameter, the audio recording interface uses the default options. For a list of keys and values you can include in the dictionary, see Audio Recording Options.

`completion`  

The block to execute when recording ends. Use this block to determine the status of the recording and to perform any cleanup. This block has no return value and takes the following parameters:

didSave  
A Boolean value indicating whether the audio was saved successfully to the specified URL. The value is true if the audio was saved or false if the user canceled the recording.

error  
An error object if a problem occurred. Use the error object to determine the cause of the problem and take any appropriate actions, such as notifying the user.

## Mentioned in 

Navigating Between Scenes

## Discussion

Use this method to obtain recorded audio from the user. This method executes asynchronously, returning shortly after you call it. During a subsequent run loop cycle, the system displays the audio recording controller to the user. The interface includes a Cancel button to dismiss the interface, and controls to manage recording. After some audio has been recorded, the interface displays the title string specified in the WKAudioRecorderControllerOptionsActionTitleKey option so that the user can accept the content and save it to the specified URL. When the user taps the Cancel button or your title string, WatchKit automatically dismisses the audio recording interface controller.

When the user dismisses the interface, or when you dismiss it programmatically, the system calls your completion block. Use that block to process the results.

Always call this method from your WatchKit extension’s main thread.

When specifying a filename with the `.wav` extension, the resulting audio format is LPCM. For all other file types, the audio format is AAC. For information about the audio recording options, see the values for WKAudioRecorderPreset.

Note

Do not attempt to record audio while gathering heart rate data using Health Kit. If you present a media interface, WatchKit automatically disables the gathering of heart rate data.

## See Also

### Presenting video and audio interfaces

func presentMediaPlayerController(with: URL, options: [AnyHashable : Any]?, completion: (Bool, TimeInterval, (any Error)?) -> Void)

Displays a modal interface for playing the specified media file.

Media Player Options

Keys indicating media playback options.

func dismissMediaPlayerController()

Dismisses the media interface controller.

enum WKAudioRecorderPreset

Constants indicating the quality of audio recordings.

Audio Recording Options

Options to specify when recording audio.

func dismissAudioRecorderController()

Dismisses the audio recording interface controller.

