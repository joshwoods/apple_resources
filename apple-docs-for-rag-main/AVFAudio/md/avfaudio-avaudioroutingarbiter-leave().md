

- AVFAudio
- AVAudioRoutingArbiter
-  leave() 

Instance Method

# leave()

Stops an app’s participation in audio routing arbitration.

macOS 11.0+

``` source
func leave()
```

## Discussion

Configure your app to notify the system when the app stops using audio for an undetermined duration. For example, for a Voice over IP (VoIP) app, call this method when the VoIP call ends. Calling this method allows the system to make an informed decision when multiple Apple devices are trying to take ownership of a Bluetooth audio route.

## See Also

### Participating in AirPods Automatic Switching

func begin(category: AVAudioRoutingArbiter.Category, completionHandler: (Bool, (any Error)?) -> Void)

Begins routing arbitration to take ownership of a nearby Bluetooth audio route.

enum Category

Categories that describe the general nature of your app’s audio use.

