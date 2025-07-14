

- Authentication Services
- ASAuthorizationPublicKeyCredentialAssertion
-  rawAuthenticatorData 

Instance Property

# rawAuthenticatorData

A byte sequence that contains additional information about the credential.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var rawAuthenticatorData: Data! { get }
```

**Required**

## Discussion

This authenticator data object contains additional information about the credential. To learn more, see the W3C Web Authentication specification.

## See Also

### Getting the properties

var signature: Data!

The signature for the assertion.

**Required**

var userID: Data!

A user identifier for the assertion.

**Required**

