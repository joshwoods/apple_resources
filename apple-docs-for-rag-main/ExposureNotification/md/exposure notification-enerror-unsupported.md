

- Exposure Notification
- ENError
-  unsupported 

Type Property

# unsupported

Operation is not supported.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
static var unsupported: ENError.Code { get }
```

## See Also

### Error Codes

static var apiMisuse: ENError.Code

The API use is incorrect.

static var badFormat: ENError.Code

A file is formated incorrectly.

static var badParameter: ENError.Code

The parameter is missing or incorrect.

static var bluetoothOff: ENError.Code

Bluetooth is turned off.

static var insufficientMemory: ENError.Code

The memory is insufficient to perform the operation.

static var insufficientStorage: ENError.Code

The storage is insufficient to enable notifications.

static var `internal`: ENError.Code

A bug in the internal notification framework.

static var invalidated: ENError.Code

A call to invalidate before the operation completes normally.

static var notAuthorized: ENError.Code

The user has denied access to the notification framework.

static var notEnabled: ENError.Code

Notification is not enabled.

static var notEntitled: ENError.Code

Process of calling is not entitled.

static var rateLimited: ENError.Code

API calls are too frequent.

static var restricted: ENError.Code

Exposure notification is disabled due to system policies.

static var unknown: ENError.Code

Failure has an unknown cause.

static var dataInaccessible: ENError.Code

The user must unlock the device before it can access data.

