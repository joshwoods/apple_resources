

- Push to Talk
- PTChannelManagerDelegate
-  channelManager(\_:didActivate:) 

Instance Method

# channelManager(\_:didActivate:)

Tells the observer the audio session activated.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func channelManager(
    _ channelManager: PTChannelManager,
    didActivate audioSession: AVAudioSession
)
```

**Required**

## Parameters 

`channelManager`  

The channel manager.

`audioSession`  

The audio session that activated.

## Mentioned in 

Creating a Push to Talk app

## Discussion

Before recording and transmitting audio, wait for the framework to call this method. The framework calls the method when the audio session is active and set to the correct priority, and allows for recording audio even if the app is in the background. The framework doesn’t call the method if the channel transmission mode is PTTransmissionMode.fullDuplex, and already has an active audio session because it’s receiving audio from a remote participant when a transmission begins.

## See Also

### Activating and deactivating the audio session

func channelManager(PTChannelManager, didDeactivate: AVAudioSession)

Tells the observer the audio session deactivated.

**Required**

