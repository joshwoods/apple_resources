

- Authentication Services
- ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest
-  excludedCredentials 

Instance Property

# excludedCredentials

An array of excluded parameters for the credential.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var excludedCredentials: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor] { get set }
```

## See Also

### Getting the properties

var credentialParameters: [ASAuthorizationPublicKeyCredentialParameters]

An array of parameters for the credential.

var residentKeyPreference: ASAuthorizationPublicKeyCredentialResidentKeyPreference

The preference that indicates where the resident key resides.

