

- Authentication Services
- ASAuthorizationPublicKeyCredentialPRFAssertionInput
-  perCredentialInputValues(\_:) 

Type Method

# perCredentialInputValues(\_:)

The inputs for the PRF extension, when not specifying general input values.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func perCredentialInputValues(_ perCredentialInputValues: [Data : ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues]) -> ASAuthorizationPublicKeyCredentialPRFAssertionInput
```

## Parameters 

`perCredentialInputValues`  

This dictionary maps `credentialID`s to input values. If the user selects a passkey with a `credentialID` that matches one of these keys, the corresponding input values will be used. If the selected passkey does not match, no PRF result will be returned. When using this option, the dictionary must be non-empty and the request must use `allowedCredentials`.

## Return Value

A configured instance of `ASAuthorizationPublicKeyCredentialPRFAssertionInput`.

