

- HomeKit
- HMError
-  notificationAlreadyEnabled 

Type Property

# notificationAlreadyEnabled

An error indicating the notification is already enabled.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var notificationAlreadyEnabled: HMError.Code { get }
```

## See Also

### Detecting general errors

static var alreadyExists: HMError.Code

An error indicating the container already contains the object you are trying to add.

static var genericError: HMError.Code

An error that does not have a more specific error code.

static var incompatibleHomeHub: HMError.Code

No compatible home hub found.

Deprecated

static var invalidClass: HMError.Code

An attempt to use an abstract base class in an operation instead of a concrete subclass.

static var notFound: HMError.Code

An error indicating the object was not found in the container.

static var notificationNotSupported: HMError.Code

An attempt to register for notifications from an accessory that does not support notifications.

static var operationNotSupported: HMError.Code

An attempt to use an unsupported operation.

static var unexpectedError: HMError.Code

An unexpected error.

static var missingEntitlement: HMError.Code

An error indicating a required entitlement is not available.

static var referToUserManual: HMError.Code

An error described in the device’s user manual.

