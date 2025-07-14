

- Authentication Services
- ASAccountAuthenticationModificationExtensionContext
-  completeChangePasswordRequest(updatedCredential:userInfo:) 

Instance Method

# completeChangePasswordRequest(updatedCredential:userInfo:)

Completes a request to update an account’s authentication credentials from using a weak password to using a strong password.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func completeChangePasswordRequest(
    updatedCredential: ASPasswordCredential,
    userInfo: [AnyHashable : Any]? = nil
)
```

## Parameters 

`updatedCredential`  

The new credentials to store in the user’s keychain.

`userInfo`  

A dictionary that contains details to pass to the extension’s containing app if the app initiated the account modification request.

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Discussion

To receive the `userInfo` dictionary in your app, set a delegate on the ASAccountAuthenticationModificationController when initiating the request. The delegate receives the `userInfo` dictionary as a parameter to accountAuthenticationModificationController(_:didSuccessfullyComplete:userInfo:).

## See Also

### Handling Requests

func completeUpgradeToSignInWithApple(userInfo: [AnyHashable : Any]?)

Completes the process of upgrading an account’s authentication credentials from using passwords to using Sign in with Apple.

func getSignInWithAppleUpgradeAuthorization(state: String?, nonce: String?, completionHandler: (ASAuthorizationAppleIDCredential?, (any Error)?) -> Void)

Retrieves the user’s current Sign in with Apple authorization credentials.

func cancelRequest(withError: any Error)

Cancels a request with an error.

let ASExtensionLocalizedFailureReasonErrorKey: String

A key that specifies a string value to show to the user when a request fails.

