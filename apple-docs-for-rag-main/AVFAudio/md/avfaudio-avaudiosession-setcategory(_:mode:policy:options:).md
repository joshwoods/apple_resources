

- AVFAudio
- AVAudioSession
-  setCategory(\_:mode:policy:options:) 

Instance Method

# setCategory(\_:mode:policy:options:)

Sets the session category, mode, route-sharing policy, and options.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 5.0+

``` source
func setCategory(
    _ category: AVAudioSession.Category,
    mode: AVAudioSession.Mode,
    policy: AVAudioSession.RouteSharingPolicy,
    options: AVAudioSession.CategoryOptions = []
) throws
```

## Parameters 

`category`  

The category to apply to the audio session. See AVAudioSession.Category for supported category values.

`mode`  

The audio session mode to apply to the audio session. For a list of values, see AVAudioSession.Mode.

`policy`  

The route-sharing policy to apply to the audio session. For a list of values, see AVAudioSession.RouteSharingPolicy.

`options`  

A mask of additional options for handling audio. For a list of constants, see AVAudioSession.CategoryOptions.

## Discussion

You specify options only with a default routing policy. With a long-form route-sharing policy, you can use the playback category and the default, moviePlayback, and spokenAudio modes.

## See Also

### Configuring standard audio behaviors

func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, options: AVAudioSession.CategoryOptions) throws

Sets the audio session’s category, mode, and options.

func setCategory(AVAudioSession.Category, options: AVAudioSession.CategoryOptions) throws

Sets the audio session’s category with the specified options.

func setCategory(AVAudioSession.Category) throws

Sets the audio session’s category.

func setMode(AVAudioSession.Mode) throws

Sets the audio session’s mode.

