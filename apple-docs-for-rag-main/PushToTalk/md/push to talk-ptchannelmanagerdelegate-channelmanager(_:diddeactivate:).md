

- Push to Talk
- PTChannelManagerDelegate
-  channelManager(\_:didDeactivate:) 

Instance Method

# channelManager(\_:didDeactivate:)

Tells the observer the audio session deactivated.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func channelManager(
    _ channelManager: PTChannelManager,
    didDeactivate audioSession: AVAudioSession
)
```

**Required**

## Parameters 

`channelManager`  

The channel manager.

`audioSession`  

The audio session that deactivated.

## Mentioned in 

Creating a Push to Talk app

## See Also

### Activating and deactivating the audio session

func channelManager(PTChannelManager, didActivate: AVAudioSession)

Tells the observer the audio session activated.

**Required**

