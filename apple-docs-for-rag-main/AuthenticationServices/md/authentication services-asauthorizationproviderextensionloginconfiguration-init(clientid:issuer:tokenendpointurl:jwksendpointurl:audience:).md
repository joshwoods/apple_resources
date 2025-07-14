

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  init(clientID:issuer:tokenEndpointURL:jwksEndpointURL:audience:) 

Initializer

# init(clientID:issuer:tokenEndpointURL:jwksEndpointURL:audience:)

Creates a configuration with the required values.

macOS 13.0+

``` source
init(
    clientID: String,
    issuer: String,
    tokenEndpointURL: URL,
    jwksEndpointURL: URL,
    audience: String?
)
```

## Parameters 

`clientID`  

The OAuth `client_id` for the login.

`issuer`  

The OAuth `issuer` for validating the token.

`tokenEndpointURL`  

The token endpoint for login.

`jwksEndpointURL`  

The URL that retrieves the JSON Web Key Set (JWKS).

`audience`  

The OAuth `audence` for embedded assertions.

## See Also

### Creating the configuration

class func configuration(openIDConfigurationURL: URL, clientID: String, issuer: String?, completion: (ASAuthorizationProviderExtensionLoginConfiguration?, (any Error)?) -> Void)

Creates a login configuration using the OpenID configuration.

