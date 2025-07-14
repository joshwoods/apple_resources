

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  invalidCredentialPredicate 

Instance Property

# invalidCredentialPredicate

The predicate string that identifies invalid credential errors.

macOS 13.0+

``` source
var invalidCredentialPredicate: String? { get set }
```

## Mentioned in 

Creating a JSON Web Encryption (JWE) login response

## Discussion

If the server returns an HTTP 400 or HTTP 401 error when authenticating, the system uses this predicate on the response body JSON. It then determines whether the error is due to an invalid password. If this predicate is `nil`, an HTTP 401 error indicates an invalid credential.

## See Also

### Obtaining the recommended configuration

var accountDisplayName: String?

The display name for the account.

