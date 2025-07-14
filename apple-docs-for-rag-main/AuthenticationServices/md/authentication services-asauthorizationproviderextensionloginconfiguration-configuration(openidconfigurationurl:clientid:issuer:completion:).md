

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  configuration(openIDConfigurationURL:clientID:issuer:completion:) 

Type Method

# configuration(openIDConfigurationURL:clientID:issuer:completion:)

Creates a login configuration using the OpenID configuration.

macOS 13.0+

``` source
class func configuration(
    openIDConfigurationURL: URL,
    clientID: String,
    issuer: String?,
    completion: @escaping (ASAuthorizationProviderExtensionLoginConfiguration?, (any Error)?) -> Void
)
```

``` source
class func configuration(
    openIDConfigurationURL: URL,
    clientID: String,
    issuer: String?
) async throws -> ASAuthorizationProviderExtensionLoginConfiguration
```

## Parameters 

`openIDConfigurationURL`  

The base URL to retrieve the `/.well-known/openid-configuration` file.

`clientID`  

The `client_id` for the Apple platform SSO login at the identity provider.

`issuer`  

The `issuer` for the requests that validate responses.

`completion`  

The completion block the system calls upon completion or error.

## See Also

### Creating the configuration

init(clientID: String, issuer: String, tokenEndpointURL: URL, jwksEndpointURL: URL, audience: String?)

Creates a configuration with the required values.

