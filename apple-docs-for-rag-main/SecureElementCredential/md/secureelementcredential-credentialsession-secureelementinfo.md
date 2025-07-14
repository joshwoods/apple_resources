

- SecureElementCredential
- CredentialSession
-  secureElementInfo 

Instance Property

# secureElementInfo

A property that provides information about the Secure Element hardware.

iOS 18.4+iPadOS 18.4+

``` source
var secureElementInfo: CredentialSession.SecureElementInfo { get async throws }
```

## Discussion

You can use the certificate in the CredentialSession.SecureElementInfo to authenticate against the Certification Authority of the Secure Element hardware.

## See Also

### Accessing hardware information

struct SecureElementInfo

A type that provides information about the Secure Element hardware.

