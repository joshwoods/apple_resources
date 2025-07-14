

- Authentication Services
- ASAuthorizationPublicKeyCredentialPRFAssertionInput
-  perCredentialInputValues 

Instance Property

# perCredentialInputValues

A map of `credentialID`s to input values for the PRF extension. If the user selects a passkey which matches a `credentialID` in this dictionary, the corresponding input values will be used. If the selected passkey does not match and `inputValues` is non-nil, that will be used instead. Otherwise, no PRF output will be returned. When this value is non-empty, the request must specify `allowedCredentials`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
let perCredentialInputValues: [Data : ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues]?
```

