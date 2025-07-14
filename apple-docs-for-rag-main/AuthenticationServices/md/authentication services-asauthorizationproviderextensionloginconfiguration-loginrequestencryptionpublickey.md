

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  loginRequestEncryptionPublicKey 

Instance Property

# loginRequestEncryptionPublicKey

macOS 14.0+

``` source
unowned(unsafe) var loginRequestEncryptionPublicKey: SecKey? { get set }
```

## Mentioned in 

Creating an encrypted embedded assertion

Creating and validating a login request

## See Also

### Instance Properties

var additionalAuthorizationScopes: String?

var customFederationUserPreauthenticationRequestValues: [URLQueryItem]

var customKeyExchangeRequestValues: [URLQueryItem]

var customKeyRequestValues: [URLQueryItem]

var customRefreshRequestValues: [URLQueryItem]

var customRequestJWTParameterName: String?

var deviceContext: Data?

var federationMEXURL: URL?

var federationMEXURLKeypath: String?

var federationPredicate: String?

var federationRequestURN: String?

var federationType: ASAuthorizationProviderExtensionLoginConfiguration.FederationType

var federationUserPreauthenticationURL: URL?

var groupRequestClaimName: String?

var groupResponseClaimName: String?

