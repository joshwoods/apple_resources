

- AVFAudio
- AVAudioSession
-  setCategory(\_:mode:options:) 

Instance Method

# setCategory(\_:mode:options:)

Sets the audio session’s category, mode, and options.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func setCategory(
    _ category: AVAudioSession.Category,
    mode: AVAudioSession.Mode,
    options: AVAudioSession.CategoryOptions = []
) throws
```

## Parameters 

`category`  

The category to apply to the audio session. See AVAudioSession.Category for supported category values.

`mode`  

The audio session mode to apply to the audio session. For a list of values, see AVAudioSession.Mode.

`options`  

A mask of additional options for handling audio. For a list of constants, see AVAudioSession.CategoryOptions.

## Discussion

The audio session’s category and mode together define how your app uses audio. Typically, you set the category and mode before activating the session. You can also set the category or mode while the session is active, but doing so results in an immediate change.

## See Also

### Configuring standard audio behaviors

func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, policy: AVAudioSession.RouteSharingPolicy, options: AVAudioSession.CategoryOptions) throws

Sets the session category, mode, route-sharing policy, and options.

func setCategory(AVAudioSession.Category, options: AVAudioSession.CategoryOptions) throws

Sets the audio session’s category with the specified options.

func setCategory(AVAudioSession.Category) throws

Sets the audio session’s category.

func setMode(AVAudioSession.Mode) throws

Sets the audio session’s mode.

