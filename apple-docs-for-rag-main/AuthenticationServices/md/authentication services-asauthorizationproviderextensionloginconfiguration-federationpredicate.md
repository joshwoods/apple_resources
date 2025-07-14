

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  federationPredicate 

Instance Property

# federationPredicate

macOS 13.3+

``` source
var federationPredicate: String? { get set }
```

## Mentioned in 

Performing a preauthentication request

Configuring authentication with the identity provider (IdP)

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

var federationRequestURN: String?

var federationType: ASAuthorizationProviderExtensionLoginConfiguration.FederationType

var federationUserPreauthenticationURL: URL?

var groupRequestClaimName: String?

var groupResponseClaimName: String?

var jwksTrustedRootCertificates: [SecCertificate]

