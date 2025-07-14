

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  federationMEXURL 

Instance Property

# federationMEXURL

macOS 13.3+

``` source
var federationMEXURL: URL? { get set }
```

## Mentioned in 

Performing a preauthentication request

Performing a WS-Trust metadata exchange data (MEX) request

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

var federationMEXURLKeypath: String?

var federationPredicate: String?

var federationRequestURN: String?

var federationType: ASAuthorizationProviderExtensionLoginConfiguration.FederationType

var federationUserPreauthenticationURL: URL?

var groupRequestClaimName: String?

var groupResponseClaimName: String?

var jwksTrustedRootCertificates: [SecCertificate]

