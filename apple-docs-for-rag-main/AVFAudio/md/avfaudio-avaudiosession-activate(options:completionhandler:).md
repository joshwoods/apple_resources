

- AVFAudio
- AVAudioSession
-  activate(options:completionHandler:) 

Instance Method

# activate(options:completionHandler:)

Activates an audio session asynchronously on watchOS.

watchOS 5.0+

``` source
func activate(
    options: AVAudioSessionActivationOptions = [],
    completionHandler handler: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func activate(options: AVAudioSessionActivationOptions = []) async throws -> Bool
```

## Parameters 

`options`  

The options to apply when activating the session.

`handler`  

The callback the system invokes when the operation completes.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func activate(options: AVAudioSessionActivationOptions = []) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to play long-form audio—such as music, podcasts, or audio books—on Apple Watch. Before calling this method to activate longform playback, you must call setCategory(_:mode:policy:options:), set the category to playback, and route sharing policy to longForm.

This method asynchronously activates the audio session. The system calls the completion handler as soon as the session has successfully activated or if the activation fails.

Playback of long-form audio on watchOS requires a Bluetooth audio route. If necessary, the system presents an audio route picker to the user, letting them choose the Bluetooth route. If the user has previously selected a Bluetooth route or if AirPods or other W1-equipped Bluetooth headphones are nearby, the system automatically picks the audio route without displaying a picker view to the user. If no applicable Bluetooth route is selected (either automatically or by the user), the system passes an error to the completion handler.

Note

You may use the activate(options:completionHandler:) method instead of the setActive(_:options:) method to authorize other categories and sharing policies. The system only presents the audio route picker for the playback category and longForm route sharing policy.

## See Also

### Activating the audio configuration

func setActive(Bool, options: AVAudioSession.SetActiveOptions) throws

Activates or deactivates your app’s audio session using the specified options.

struct AVAudioSessionActivationOptions

Constants that describe the options to pass when activating the audio session.

