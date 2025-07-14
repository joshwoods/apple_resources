

- Push to Talk
- PTChannelError
-  channelNotFound 

Type Property

# channelNotFound

A channel error that indicates the system can’t perform the action because there’s no active channel with the UUID you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static var channelNotFound: PTChannelError.Code { get }
```

## See Also

### Constants

static var unknown: PTChannelError.Code

A channel error that indicates an unknown error.

static var appNotForeground: PTChannelError.Code

A channel error that indicates the operation failed because the app isn’t in the foreground.

static var channelLimitReached: PTChannelError.Code

A channel error that indicates you reached the maximum of one active channel at a time for the entire device.

static var callActive: PTChannelError.Code

A channel error that indicates there’s an active call that prevents the channel action.

static var transmissionInProgress: PTChannelError.Code

A channel error that indicates a transmission is already in progress.

static var transmissionNotFound: PTChannelError.Code

A channel error that indicates there’s no transmission to stop.

static var deviceManagementRestriction: PTChannelError.Code

A channel error that indicates a device-management policy or profile forbids joining the channel.

static var screenTimeRestriction: PTChannelError.Code

A channel error that indicates a Screen Time restriction prevents the action.

static var transmissionNotAllowed: PTChannelError.Code

A channel error that indicates the current transmission mode of the channel doesn’t allow the mode you specify.

