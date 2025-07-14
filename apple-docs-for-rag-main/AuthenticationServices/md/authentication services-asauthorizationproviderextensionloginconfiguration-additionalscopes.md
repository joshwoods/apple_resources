

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  additionalScopes 

Instance Property

# additionalScopes

A set of extra scopes to add to the base for the authentication request.

macOS 13.0+

``` source
var additionalScopes: String { get set }
```

## Mentioned in 

Creating an embedded assertion

Creating a refresh request

Creating an encrypted embedded assertion

Creating and validating a login request

## Discussion

The base value is `openid offline_access`. The system appends any additional values. The default additional scope is `urn:apple:platformsso`.

## See Also

### Customizing the authentication request

func setCustomAssertionRequestBodyClaims([String : Any]) throws

Adds the custom claims to the embedded assertion request body.

func setCustomAssertionRequestHeaderClaims([String : Any]) throws

Adds the custom claims to the embedded assertion request header.

func setCustomLoginRequestBodyClaims([String : Any]) throws

Adds the custom claims to the login request body.

func setCustomLoginRequestHeaderClaims([String : Any]) throws

Adds the custom claims to the login request header.

var customLoginRequestValues: [URLQueryItem]

Provider-supplied values to add to the login POST request body.

var kerberosTicketMappings: [ASAuthorizationProviderExtensionKerberosMapping]

The set of ticket mappings the system uses to import Kerberos tickets from the single sign-on token.

