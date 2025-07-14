

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  customLoginRequestValues 

Instance Property

# customLoginRequestValues

Provider-supplied values to add to the login POST request body.

macOS 13.0+

``` source
var customLoginRequestValues: [URLQueryItem] { get set }
```

## Mentioned in 

Creating and validating a login request

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

var additionalScopes: String

A set of extra scopes to add to the base for the authentication request.

var kerberosTicketMappings: [ASAuthorizationProviderExtensionKerberosMapping]

The set of ticket mappings the system uses to import Kerberos tickets from the single sign-on token.

