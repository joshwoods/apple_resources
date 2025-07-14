

- Authentication Services
- ASAuthorizationPublicKeyCredentialPRFAssertionInput
- ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues
-  saltInput1(\_:saltInput2:) 

Type Method

# saltInput1(\_:saltInput2:)

The inputs for generating the PRF output secrets.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func saltInput1(
    _ saltInput1: Data,
    saltInput2: Data? = nil
) -> ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues
```

## Parameters 

`saltInput1`  

The input used when generating `first`.

`saltInput2`  

If specified, the input when generating `second`. If not specified, `second` will be nil.

## Return Value

A configured instance of `InputValues`.

