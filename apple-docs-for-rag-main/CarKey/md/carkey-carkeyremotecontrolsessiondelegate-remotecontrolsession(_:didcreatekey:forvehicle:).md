

- CarKey
- CarKeyRemoteControlSessionDelegate
-  remoteControlSession(\_:didCreateKey:forVehicle:) 

Instance Method

# remoteControlSession(\_:didCreateKey:forVehicle:)

Called to notify your app when a new key has been created.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
func remoteControlSession(
    _ session: CarKeyRemoteControlSession,
    didCreateKey keyID: String,
    forVehicle vehicleID: String
)
```

**Required** Default implementation provided.

## Parameters 

`session`  

The current session.

`keyID`  

The identifier of the key.

`vehicleID`  

The identifier of the vehicle.

## Default Implementations

### CarKeyRemoteControlSessionDelegate Implementations

func remoteControlSession(CarKeyRemoteControlSession, didCreateKey: String, forVehicle: String)

Called to notify your app when a new key has been created.

