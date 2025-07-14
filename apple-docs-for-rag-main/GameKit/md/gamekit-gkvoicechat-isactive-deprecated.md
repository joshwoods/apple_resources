

- GameKit
- GKVoiceChat
-  isActive Deprecated

Instance Property

# isActive

A Boolean value that indicates whether the channel is sampling the microphone.

iOS 4.1–18.0DeprecatediPadOS 4.1–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var isActive: Bool { get set }
```

Deprecated

No longer supported

## Mentioned in 

Adding voice chat to multiplayer games

## Discussion

If you set this property to true, the voice chat object transmits the voice data from the microphone to other players in the channel. If another voice chat object is using the microphone, GameKit switches the microphone to this channel and sets that voice chat object’s isActive property to false.

The default value for this property is false.

## See Also

### Starting and Stopping Voice Chat

func start()

Starts communication with other players in a channel.

Deprecated

func stop()

Ends communication with other players in a channel.

Deprecated

