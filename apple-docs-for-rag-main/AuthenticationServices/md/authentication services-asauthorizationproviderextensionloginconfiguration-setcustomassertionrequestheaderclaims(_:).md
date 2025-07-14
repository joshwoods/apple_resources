

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  setCustomAssertionRequestHeaderClaims(\_:) 

Instance Method

# setCustomAssertionRequestHeaderClaims(\_:)

Adds the custom claims to the embedded assertion request header.

macOS 13.0+

``` source
func setCustomAssertionRequestHeaderClaims(_ claims: [String : Any]) throws
```

## Parameters 

`claims`  

The claims to add. The request must serialize as valid JSON for the system to accept it.

## See Also

### Customizing the authentication request

func setCustomAssertionRequestBodyClaims([String : Any]) throws

Adds the custom claims to the embedded assertion request body.

func setCustomLoginRequestBodyClaims([String : Any]) throws

Adds the custom claims to the login request body.

func setCustomLoginRequestHeaderClaims([String : Any]) throws

Adds the custom claims to the login request header.

var additionalScopes: String

A set of extra scopes to add to the base for the authentication request.

var customLoginRequestValues: [URLQueryItem]

Provider-supplied values to add to the login POST request body.

var kerberosTicketMappings: [ASAuthorizationProviderExtensionKerberosMapping]

The set of ticket mappings the system uses to import Kerberos tickets from the single sign-on token.

