

- Authentication Services
- ASAuthorizationPublicKeyCredentialPRFRegistrationOutput
-  init(first:second:) 

Initializer

# init(first:second:)

This method should only be called if input values were provided with the registration request. Otherwise, use `.supported` or `.unsupported`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    first: SymmetricKey,
    second: SymmetricKey?
)
```

