

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  federationType 

Instance Property

# federationType

macOS 13.3+

``` source
var federationType: ASAuthorizationProviderExtensionLoginConfiguration.FederationType { get set }
```

## Mentioned in 

Configuring authentication with the identity provider (IdP)

Performing a WS-Trust metadata exchange data (MEX) request

Performing a preauthentication request

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

var federationUserPreauthenticationURL: URL?

var groupRequestClaimName: String?

var groupResponseClaimName: String?

var jwksTrustedRootCertificates: [SecCertificate]

