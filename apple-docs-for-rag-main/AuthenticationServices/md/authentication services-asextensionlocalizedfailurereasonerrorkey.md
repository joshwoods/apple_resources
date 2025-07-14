

- Authentication Services
-  ASExtensionLocalizedFailureReasonErrorKey 

Global Variable

# ASExtensionLocalizedFailureReasonErrorKey

A key that specifies a string value to show to the user when a request fails.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
let ASExtensionLocalizedFailureReasonErrorKey: String
```

## Discussion

When canceling a request, your extension calls cancelRequest(withError:). The system informs the user that the request failed. To show additional information regarding the failure, use this key to set a string value in the error’s `userInfo` dictionary.

## See Also

### Handling Requests

func completeUpgradeToSignInWithApple(userInfo: [AnyHashable : Any]?)

Completes the process of upgrading an account’s authentication credentials from using passwords to using Sign in with Apple.

func completeChangePasswordRequest(updatedCredential: ASPasswordCredential, userInfo: [AnyHashable : Any]?)

Completes a request to update an account’s authentication credentials from using a weak password to using a strong password.

func getSignInWithAppleUpgradeAuthorization(state: String?, nonce: String?, completionHandler: (ASAuthorizationAppleIDCredential?, (any Error)?) -> Void)

Retrieves the user’s current Sign in with Apple authorization credentials.

func cancelRequest(withError: any Error)

Cancels a request with an error.

