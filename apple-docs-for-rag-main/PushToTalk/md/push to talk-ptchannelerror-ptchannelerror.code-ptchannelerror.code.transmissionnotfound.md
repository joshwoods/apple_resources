

- Push to Talk
- PTChannelError
- PTChannelError.Code
-  PTChannelError.Code.transmissionNotFound 

Case

# PTChannelError.Code.transmissionNotFound

A channel error that indicates there’s no transmission to stop.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
case transmissionNotFound
```

## See Also

### Error codes

case unknown

A channel error that indicates an unknown error.

case appNotForeground

A channel error that indicates the operation failed because the app isn’t in the foreground.

case channelNotFound

A channel error that indicates the system can’t perform the action because there’s no active channel with the UUID you specify.

case channelLimitReached

A channel error that indicates you reached the maximum of one active channel at a time for the entire device.

case callActive

A channel error that indicates there’s an active call that prevents the channel action.

case transmissionInProgress

A channel error that indicates a transmission is already in progress.

case deviceManagementRestriction

A channel error that indicates a device-management policy or profile forbids joining the channel.

case screenTimeRestriction

A channel error that indicates a Screen Time restriction prevents the action.

case transmissionNotAllowed

A channel error that indicates the current transmission mode of the channel doesn’t allow the mode you specify.

