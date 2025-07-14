

- CarKey
- CarKeyErrorCode
-  CarKeyErrorCode.VehicleNotConnected 

Case

# CarKeyErrorCode.VehicleNotConnected

An error that indicates the vehicle isn’t available to respond to the request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
case VehicleNotConnected
```

## Discussion

Make sure you are in range of the vehicle and that the isConnected property of the vehicle report is `true`.

## See Also

### Getting the Error Code

case AnotherRequestInProgress

An error that indicates a previous request is still in progress.

case ClientInBackground

An error that indicates the operation occurred when the app was in the background.

case EnduringRequestUsingEventMethod

An error that indicates a mismatch between the initial request type and the results.

case FeatureNotSupported

An error that indicates the specified feature isn’t supported in the current environment.

case FunctionUnknown

An error that indicates the vehicle didn’t recognize the specified function identifier.

case Internal

An error that indicates an unknown error occurred.

case MessageTooLong

An error that indicates the command you sent was too long.

case RequestNotInProgress

An error that indicates an enduring operation wasn’t running.

case RequestTimedOut

An error that indicates the request didn’t complete in time.

case SecurityViolation

An error that indicates your app doesn’t have the required entitlements.

case SessionNotActive

An error that indicates an active session is currently inactive.

case VehicleNotFound

An error that indicates a vehicle with the specified ID wasn’t found.

