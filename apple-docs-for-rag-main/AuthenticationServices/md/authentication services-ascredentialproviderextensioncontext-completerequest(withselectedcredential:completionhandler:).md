

- Authentication Services
- ASCredentialProviderExtensionContext
-  completeRequest(withSelectedCredential:completionHandler:) 

Instance Method

# completeRequest(withSelectedCredential:completionHandler:)

Provides the user-selected credential.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func completeRequest(
    withSelectedCredential credential: ASPasswordCredential,
    completionHandler: ((Bool) -> Void)? = nil
)
```

## Parameters 

`credential`  

The credential that the user selected.

`completionHandler`  

Optional work that the extension performs as a background priority task after the request completes. The `expired` parameter is `YES` if the system prematurely terminates a previous non-expiration invocation of the `completionHandler`.

## Discussion

After calling this method, the system dismisses the associated view controller.

## See Also

### Providing credentials

func completeAssertionRequest(using: ASPasskeyAssertionCredential, completionHandler: ((Bool) -> Void)?)

Complete the passkey assertion request by providing the user-selected passkey credential.

func completeRegistrationRequest(using: ASPasskeyRegistrationCredential, completionHandler: ((Bool) -> Void)?)

Complete the registration request by providing the newly-created passkey credential.

func completeOneTimeCodeRequest(using: ASOneTimeCodeCredential, completionHandler: ((Bool) -> Void)?)

Provides the user-selected one-time passcode (OTP).

class ASPasswordCredential

A password credential.

class ASPasskeyAssertionCredential

A passkey assertion credential.

class ASPasskeyRegistrationCredential

A passkey registration credential.

class ASOneTimeCodeCredential

A one-time passcode (OTP) credential.

