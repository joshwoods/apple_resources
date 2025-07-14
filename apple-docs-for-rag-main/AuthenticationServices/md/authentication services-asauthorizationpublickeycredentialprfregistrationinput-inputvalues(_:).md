

- Authentication Services
- ASAuthorizationPublicKeyCredentialPRFRegistrationInput
-  inputValues(\_:) 

Type Method

# inputValues(\_:)

The inputs for the PRF extension, to evaluate if the new passkey supports this extension.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func inputValues(_ inputValues: ASAuthorizationPublicKeyCredentialPRFRegistrationInput.InputValues) -> ASAuthorizationPublicKeyCredentialPRFRegistrationInput
```

## Parameters 

`inputValues`  

These are the inputs that will be used for generating the PRF.

## Return Value

A configured instance of `ASAuthorizationPublicKeyCredentialPRFRegistrationInput`.

