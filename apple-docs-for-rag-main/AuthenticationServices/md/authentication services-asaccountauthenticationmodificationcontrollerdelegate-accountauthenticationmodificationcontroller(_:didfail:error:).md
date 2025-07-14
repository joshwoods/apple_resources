

- Authentication Services
- ASAccountAuthenticationModificationControllerDelegate
-  accountAuthenticationModificationController(\_:didFail:error:) 

Instance Method

# accountAuthenticationModificationController(\_:didFail:error:)

Tells the delegate an account modification request failed.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
optional func accountAuthenticationModificationController(
    _ controller: ASAccountAuthenticationModificationController,
    didFail request: ASAccountAuthenticationModificationRequest,
    error: any Error
)
```

## Parameters 

`controller`  

The account authentication modification controller that initiated the request.

`request`  

The request that failed.

`error`  

An error that indicates why the request failed.

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## See Also

### Handling Requests

func accountAuthenticationModificationController(ASAccountAuthenticationModificationController, didSuccessfullyComplete: ASAccountAuthenticationModificationRequest, userInfo: [AnyHashable : Any]?)

Tells the delegate an account modification request completed successfully.

