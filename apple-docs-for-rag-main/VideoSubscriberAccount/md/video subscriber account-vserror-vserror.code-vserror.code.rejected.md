

- Video Subscriber Account
- VSError
- VSError.Code
-  VSError.Code.rejected 

Case

# VSError.Code.rejected

The system rejected the request.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
case rejected
```

## Discussion

Only TV provider apps can use this error code.

## See Also

### Error Codes

case accessNotGranted

The user hasn’t granted access to their subscription information.

case invalidVerificationToken

The user’s subscription provider rejected the verification token that the app sent with the request.

case providerRejected

The user’s subscription provider didn’t allow the request to proceed.

case serviceTemporarilyUnavailable

The request failed due to a timeout or unreachable host, but a subsequent attempt might succeed.

case unsupported

The provider doesn’t support the feature the user requested in the device’s current region.

case unsupportedProvider

The system doesn’t support the user’s subscription provider.

case userCancelled

The user canceled the request.

