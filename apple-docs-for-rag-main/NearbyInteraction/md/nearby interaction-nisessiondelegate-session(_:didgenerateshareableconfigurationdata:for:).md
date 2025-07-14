

- Nearby Interaction
- NISessionDelegate
-  session(\_:didGenerateShareableConfigurationData:for:) 

Instance Method

# session(\_:didGenerateShareableConfigurationData:for:)

Provides configuration data to share with a third-party accessory.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+watchOS 8.0+

``` source
optional func session(
    _ session: NISession,
    didGenerateShareableConfigurationData shareableConfigurationData: Data,
    for object: NINearbyObject
)
```

## Parameters 

`session`  

The session that produced the configuration data.

`shareableConfigurationData`  

The data to share with the accessory.

`object`  

A representation of the accessory as an NINearbyObject.

## Mentioned in 

Initiating and maintaining a session

## Discussion

The system invokes this callback only for sessions that run an accessory configuration. The `shareableConfigurationData` argument contains information that the accessory needs to begin the session. For more information, see NINearbyAccessoryConfiguration.

## See Also

### Monitoring peers

func session(NISession, didUpdate: [NINearbyObject])

Notifies you when the session updates nearby objects.

func session(NISession, didRemove: [NINearbyObject], reason: NINearbyObject.RemovalReason)

Notifies you when the session removes one or more nearby objects.

enum RemovalReason

The reason a session removed a nearby object.

