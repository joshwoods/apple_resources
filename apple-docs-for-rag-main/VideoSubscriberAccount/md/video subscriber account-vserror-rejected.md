

- Video Subscriber Account
- VSError
-  rejected 

Type Property

# rejected

The system rejected the request.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
static var rejected: VSError.Code { get }
```

## Discussion

Only TV provider apps can use this error code.

## See Also

### Error Codes

static var accessNotGranted: VSError.Code

The user hasn’t granted access to their subscription information.

static var invalidVerificationToken: VSError.Code

The user’s subscription provider rejected the verification token that the app sent with the request.

static var providerRejected: VSError.Code

The user’s subscription provider didn’t allow the request to proceed.

static var serviceTemporarilyUnavailable: VSError.Code

The request failed due to a timeout or unreachable host, but a subsequent attempt might succeed.

static var unsupported: VSError.Code

The provider doesn’t support the feature the user requested in the device’s current region.

static var unsupportedProvider: VSError.Code

The system doesn’t support the user’s subscription provider.

static var userCancelled: VSError.Code

The user canceled the request.

enum Code

Error codes in the framework error domain.

