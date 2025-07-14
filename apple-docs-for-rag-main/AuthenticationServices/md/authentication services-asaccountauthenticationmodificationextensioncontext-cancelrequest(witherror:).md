

- Authentication Services
- ASAccountAuthenticationModificationExtensionContext
-  cancelRequest(withError:) 

Instance Method

# cancelRequest(withError:)

Cancels a request with an error.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func cancelRequest(withError error: any Error)
```

## Parameters 

`error`  

An error that indicates the reason for the canceled request.

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Discussion

If the user cancels the request, use the ASExtensionError.Code.userCanceled error code in the `error`. If the request requires user interaction, use ASExtensionError.Code.userInteractionRequired instead.

To include additional information regarding the failure, use ASExtensionLocalizedFailureReasonErrorKey to set a string value in the error’s `userInfo` dictionary. The system displays this string value to the user.

## See Also

### Handling Requests

func completeUpgradeToSignInWithApple(userInfo: [AnyHashable : Any]?)

Completes the process of upgrading an account’s authentication credentials from using passwords to using Sign in with Apple.

func completeChangePasswordRequest(updatedCredential: ASPasswordCredential, userInfo: [AnyHashable : Any]?)

Completes a request to update an account’s authentication credentials from using a weak password to using a strong password.

func getSignInWithAppleUpgradeAuthorization(state: String?, nonce: String?, completionHandler: (ASAuthorizationAppleIDCredential?, (any Error)?) -> Void)

Retrieves the user’s current Sign in with Apple authorization credentials.

let ASExtensionLocalizedFailureReasonErrorKey: String

A key that specifies a string value to show to the user when a request fails.

