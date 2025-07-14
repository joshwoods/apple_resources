

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  kerberosTicketMappings 

Instance Property

# kerberosTicketMappings

The set of ticket mappings the system uses to import Kerberos tickets from the single sign-on token.

macOS 13.0+

``` source
var kerberosTicketMappings: [ASAuthorizationProviderExtensionKerberosMapping] { get set }
```

## Mentioned in 

Creating a JSON Web Encryption (JWE) login response

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

var customLoginRequestValues: [URLQueryItem]

Provider-supplied values to add to the login POST request body.

