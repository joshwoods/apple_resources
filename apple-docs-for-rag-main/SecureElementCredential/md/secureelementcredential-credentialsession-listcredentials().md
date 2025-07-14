

- SecureElementCredential
- CredentialSession
-  listCredentials() 

Instance Method

# listCredentials()

Retrieves a list of of credentials to which the app has access rights.

iOS 18.1+iPadOS 18.1+

``` source
func listCredentials() async throws -> [CredentialSession.Credential]
```

## Return Value

An array of credentials to which the calling app has access rights. The order of credentials in this array is random.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

When you call this method, the framework caches a snapshot of these credentials. Because credentials can change, refresh your data models whenever your app performs any kind of write operation using the SecureElementCredential framework. Also update whenever your app returns to the foreground.

## See Also

### Accessing credentials

struct Credential

Information about a credential that a credential session retrieves from the Secure Element.

