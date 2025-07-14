

- AVFAudio
- AVAudioRoutingArbiter
-  begin(category:completionHandler:) 

Instance Method

# begin(category:completionHandler:)

Begins routing arbitration to take ownership of a nearby Bluetooth audio route.

macOS 11.0+

``` source
func begin(
    category: AVAudioRoutingArbiter.Category,
    completionHandler handler: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func begin(category: AVAudioRoutingArbiter.Category) async throws -> Bool
```

## Parameters 

`category`  

A category that describes how the app uses audio.

`handler`  

A completion handler the system calls asynchronously when the system completes audio routing arbitration. This closure takes the following parameters:

defaultDeviceChanged  
A Boolean value that indicates whether the system switched the AirPods to the macOS device.

error  
An error object that indicates why the request failed, or nil if the request succeeded.

## Discussion

Call this method to tell the operating system to arbitrate with nearby Apple devices to take ownership of a supported Bluetooth audio device. When arbitration completes, the system calls the completion handler, passing a Boolean that indicates whether the audio device changed. In either case, begin using audio as normal.

## See Also

### Participating in AirPods Automatic Switching

enum Category

Categories that describe the general nature of your app’s audio use.

func leave()

Stops an app’s participation in audio routing arbitration.

