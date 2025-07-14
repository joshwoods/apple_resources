

- AVFAudio
- AVAudioSession
-  setCategory(\_:) 

Instance Method

# setCategory(\_:)

Sets the audio session’s category.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setCategory(_ category: AVAudioSession.Category) throws
```

## Parameters 

`category`  

The category to apply to the audio session. See AVAudioSession.Category for supported category values.

## Discussion

The audio session’s category defines how the app uses audio. Typically, you set the category before activating the session. You can also set the category while the session is active, but this results in an immediate route change.

Note

Instead of setting your category and mode properties independently, set them at the same time using the setCategory(_:mode:options:) or setCategory(_:mode:policy:options:) method.

## See Also

### Configuring standard audio behaviors

func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, policy: AVAudioSession.RouteSharingPolicy, options: AVAudioSession.CategoryOptions) throws

Sets the session category, mode, route-sharing policy, and options.

func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, options: AVAudioSession.CategoryOptions) throws

Sets the audio session’s category, mode, and options.

func setCategory(AVAudioSession.Category, options: AVAudioSession.CategoryOptions) throws

Sets the audio session’s category with the specified options.

func setMode(AVAudioSession.Mode) throws

Sets the audio session’s mode.

