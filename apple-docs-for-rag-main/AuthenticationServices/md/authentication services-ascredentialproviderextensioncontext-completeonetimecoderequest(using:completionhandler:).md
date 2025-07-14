

- Authentication Services
- ASCredentialProviderExtensionContext
-  completeOneTimeCodeRequest(using:completionHandler:) 

Instance Method

# completeOneTimeCodeRequest(using:completionHandler:)

Provides the user-selected one-time passcode (OTP).

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func completeOneTimeCodeRequest(
    using credential: ASOneTimeCodeCredential,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
func completeOneTimeCodeRequest(using credential: ASOneTimeCodeCredential) async -> Bool
```

## Parameters 

`credential`  

The OTP credential chosen by the person.

`completionHandler`  

Optional work that the extension performs as a background priority task after the request completes. The `expired` parameter is `YES` if the system prematurely terminates a previous non-expiration invocation of the `completionHandler`.

## Mentioned in 

Providing one-time passcodes to AutoFill

## Overview

After calling this method, the system dismisses the associated view controller.

## See Also

### Providing credentials

func completeRequest(withSelectedCredential: ASPasswordCredential, completionHandler: ((Bool) -> Void)?)

Provides the user-selected credential.

func completeAssertionRequest(using: ASPasskeyAssertionCredential, completionHandler: ((Bool) -> Void)?)

Complete the passkey assertion request by providing the user-selected passkey credential.

func completeRegistrationRequest(using: ASPasskeyRegistrationCredential, completionHandler: ((Bool) -> Void)?)

Complete the registration request by providing the newly-created passkey credential.

class ASPasswordCredential

A password credential.

class ASPasskeyAssertionCredential

A passkey assertion credential.

class ASPasskeyRegistrationCredential

A passkey registration credential.

class ASOneTimeCodeCredential

A one-time passcode (OTP) credential.

