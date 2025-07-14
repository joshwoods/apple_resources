

- Authentication Services
- ASAccountAuthenticationModificationExtensionContext
-  getSignInWithAppleUpgradeAuthorization(state:nonce:completionHandler:) 

Instance Method

# getSignInWithAppleUpgradeAuthorization(state:nonce:completionHandler:)

Retrieves the user’s current Sign in with Apple authorization credentials.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func getSignInWithAppleUpgradeAuthorization(
    state: String?,
    nonce: String?,
    completionHandler: @escaping (ASAuthorizationAppleIDCredential?, (any Error)?) -> Void
)
```

``` source
func requestSignInWithAppleUpgradeAuthorization(
    state: String?,
    nonce: String?
) async throws -> ASAuthorizationAppleIDCredential
```

## Parameters 

`state`  

A string that contains a random value for verifying the Sign in with Apple credentials.

`nonce`  

A string that contains a random value for verifying the Sign in with Apple credentials.

`completionHandler`  

A closure that takes a parameter for the user’s current Sign in with Apple credentials, and an error if one occurs while retrieving them.

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Discussion

Calling this method causes the system to present the Sign in with Apple upgrade interface, dismissing any currently presented interface.

For more information about the `state` and `nonce` parameters, see Authenticating users with Sign in with Apple and Get the most out of Sign in with Apple.

## See Also

### Handling Requests

func completeUpgradeToSignInWithApple(userInfo: [AnyHashable : Any]?)

Completes the process of upgrading an account’s authentication credentials from using passwords to using Sign in with Apple.

func completeChangePasswordRequest(updatedCredential: ASPasswordCredential, userInfo: [AnyHashable : Any]?)

Completes a request to update an account’s authentication credentials from using a weak password to using a strong password.

func cancelRequest(withError: any Error)

Cancels a request with an error.

let ASExtensionLocalizedFailureReasonErrorKey: String

A key that specifies a string value to show to the user when a request fails.

