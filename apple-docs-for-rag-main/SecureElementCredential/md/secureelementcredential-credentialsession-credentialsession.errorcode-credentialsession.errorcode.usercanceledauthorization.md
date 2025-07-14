

- SecureElementCredential
- CredentialSession
- CredentialSession.ErrorCode
-  CredentialSession.ErrorCode.userCanceledAuthorization 

Case

# CredentialSession.ErrorCode.userCanceledAuthorization

The person using the app dismissed the authorization sheet.

iOS 18.1+iPadOS 18.1+

``` source
case userCanceledAuthorization
```

## Discussion

In this scenario, the credential session’s underlying state transitions to CredentialSession.State.management.

## See Also

### Authorization and permission error codes

case userNotAuthorized

The person using the app isn’t authorized to perform the operation.

case accessDenied

The person using the app declined to grant permission for the operation.

case clientNotInForeground

Your app isn’t in the foreground, which is required to use the credential session.

case userAuthorizationTimedOut

Authorization timed out while waiting for the person using the app.

case featureUnavailable

The feature is unavailable.

case ineligible

The current device and user configuation are ineligible to use this service.

case conditionsNotSatisfied

The iCloud account or passcode of the person using the app don’t satisfy the conditions to use this service.

