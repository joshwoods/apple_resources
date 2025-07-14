

- Authentication Services
- ASAuthorizationPublicKeyCredentialPRFAssertionInput
-  inputValues(\_:perCredentialInputValues:) 

Type Method

# inputValues(\_:perCredentialInputValues:)

The inputs for the PRF extension.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func inputValues(
    _ inputValues: ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues,
    perCredentialInputValues: [Data : ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues]? = nil
) -> ASAuthorizationPublicKeyCredentialPRFAssertionInput
```

## Parameters 

`inputValues`  

These are the default inputs that will be used for generating the PRF.

`perCredentialInputValues`  

This optional dictionary maps `credentialID`s to alternate input values. If the user selects a passkey with a `credentialID` that matches one of these keys, the corresponding input values will be used instead of those from the first argument. When specifying a non-empty value here, the request must use `allowedCredentials`.

## Return Value

A configured instance of `ASAuthorizationPublicKeyCredentialPRFAssertionInput`.

