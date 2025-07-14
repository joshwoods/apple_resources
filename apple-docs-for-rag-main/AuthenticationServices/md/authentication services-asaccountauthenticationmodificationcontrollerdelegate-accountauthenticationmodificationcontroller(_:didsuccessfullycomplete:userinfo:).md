

- Authentication Services
- ASAccountAuthenticationModificationControllerDelegate
-  accountAuthenticationModificationController(\_:didSuccessfullyComplete:userInfo:) 

Instance Method

# accountAuthenticationModificationController(\_:didSuccessfullyComplete:userInfo:)

Tells the delegate an account modification request completed successfully.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
optional func accountAuthenticationModificationController(
    _ controller: ASAccountAuthenticationModificationController,
    didSuccessfullyComplete request: ASAccountAuthenticationModificationRequest,
    userInfo: [AnyHashable : Any]? = nil
)
```

## Parameters 

`controller`  

The account authentication modification controller that initiated the request.

`request`  

The request that failed.

`userInfo`  

A dictionary that contains values from the account modification extension.

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## See Also

### Handling Requests

func accountAuthenticationModificationController(ASAccountAuthenticationModificationController, didFail: ASAccountAuthenticationModificationRequest, error: any Error)

Tells the delegate an account modification request failed.

