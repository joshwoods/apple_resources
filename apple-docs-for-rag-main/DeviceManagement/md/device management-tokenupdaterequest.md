

- Device Management
-  TokenUpdateRequest 

Device Management Command

# TokenUpdateRequest

The request object for sending the new token details.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object TokenUpdateRequest
```

## Properties

`AwaitingConfiguration`

`boolean`

If `true` from the device channel, the device is awaiting a Release Device from Await Configuration MDM command before proceeding through Setup Assistant.

If `true` from the user channel (Shared iPad only), the device is awaiting a UserConfiguredCommand MDM command before proceeding through Setup Assistant.

Default: `false`

`EnrollmentID`

`string`

 (Required) 

The per-enrollment identifier for the device. Available in macOS 10.15 and iOS 13.0 and later.

`EnrollmentUserID`

`string`

 (Required) 

The per-enrollment identifier for the user. Available in macOS 10.15 and iOS 13.0 and later.

`MessageType`

`string`

 (Required) 

The message type, which must have a value of `TokenUpdate`.

Value: `TokenUpdate`

`NotOnConsole`

`boolean`

 (Required) 

If true, the device is not on console.

`PushMagic`

`string`

 (Required) 

The magic string that has to be included in the push notification message.

`Token`

`data`

 (Required) 

The Push token for the device.

`Topic`

`string`

 (Required) 

The topic the device subscribes to.

`UDID`

`string`

 (Required) 

The device’s UDID.

`UnlockToken`

`data`

The data that can be used to unlock the device. If provided, the server should remember this data and send it with when trying to Clear the Passcode.

`UserShortName`

`string`

On Shared iPad: This is the Managed Apple ID of the user on Shared iPad. It indicates that the token is for the user channel.

On macOS, this is the short name of the user.

`UserID`

`string`

On macOS: This is the ID of the user.

On Shared iPad: This is always `FFFFFFFF-FFFF-FFFF-FFFF-FFFFFFFFFFFF` to indicate that no authentication will occur.

`UserLongName`

`string`

 (Required) 

The full name of the user.

## Mentioned in 

Managing Passcodes

## Discussion

The device sends an initial token update message to the server when it has installed the MDM payload. The server should send push messages to the device only after receiving the first token update message. If the device reports that it is `AwaitingConfiguration`, the MDM server is expected to send a Release Device from Await Configuration MDM command before the device can allow the user to proceed in Setup Assistant. This gives the MDM server the opportunity to do some setup via MDM commands.

In addition to sending the initial Token Update message, the iOS device may now send additional Token Update messages to the check-in server at any time while it has a valid MDM enrollment.

The use of `PushMagic` constrains the device to a unique MDM relationship. When a user removes the MDM profile, the device should no longer listen to the former relationship, even if the user reestablishes a management relationship with the same server topic. Note that only the push topic is the same in this case; the serverʼs address could have changed. This also helps when a user restores a device from backup that contains an older relationship. The use of `PushMagic` also ensures that the server that receives the `CheckIn` message is owned by the same enterprise as the computer sending push notifications. This is important because there is no way of knowing if the push topic belongs to the owner of the checkin server. It is conceivable that Apple could revoke a push token for one party, only to have that party re-enroll people piggybacking on some other topic thatʼs actively pushing. The fact that all MDM push topics reside in the namespace com.apple.mgmt.\* helps prevent this.

The `PushMagic` or `UnlockToken` fields of subsequent Token Update messages may be identical to those in previous messages or may be different (and may differ in size from previous values). If different, the server should update its record for the device to the new value provided by the message. Failure to do so results in the server being unable to send push notifications or perform passcode resets.

While the `UnlockToken` message can be sent multiple times by the device, it is possible it may only be sent once if `PushMagic` or `UnlockToken` values change. Implementations should not rely on repeated messages to update lost server-side data or to recover from a failure to process a previous Token Update message.

While the `Token Update` message can be sent multiple times by the device, it is possible that it may only be sent once if the values contained within the message never change. Implementations should not rely on repeated messages to update lost server-side data or to recover from a failure to process a previous `Token Update` message. Also note that the `UnlockToken` is optional. The absence of an `UnlockToken` in a `Token Update` message should not be treated as an invalidation of a previously received `UnlockToken`.

Note

The topic string for the MDM check-in protocol must start with `com.apple.mgmt.*` where `*` is a unique suffix.

