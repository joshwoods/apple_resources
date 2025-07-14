

- Audio Toolbox
- AUAudioUnit
-  messageChannel(for:) 

Instance Method

# messageChannel(for:)

Returns an object for bidirectional communication between an audio unit and its host.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func messageChannel(for channelName: String) -> any AUMessageChannel
```

## Parameters 

`channelName`  

The name of the message channel the audio unit returns.

## Return Value

An object that conforms to AUMessageChannel.

## Discussion

Message channels provide a way for custom data exchanges between an audio unit and its host. An audio unit may support multiple message channels.

The host manages the message channel object’s lifetime. Design message channel objects so they can outlive the audio unit that vended them.

## See Also

### Messaging Channels

protocol AUMessageChannel

A specification for a bidirectional communication message channel.

