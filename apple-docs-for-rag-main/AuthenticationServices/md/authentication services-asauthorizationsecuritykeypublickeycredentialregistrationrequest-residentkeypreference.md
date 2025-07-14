

- Authentication Services
- ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest
-  residentKeyPreference 

Instance Property

# residentKeyPreference

The preference that indicates where the resident key resides.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var residentKeyPreference: ASAuthorizationPublicKeyCredentialResidentKeyPreference { get set }
```

## See Also

### Getting the properties

var credentialParameters: [ASAuthorizationPublicKeyCredentialParameters]

An array of parameters for the credential.

var excludedCredentials: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor]

An array of excluded parameters for the credential.

