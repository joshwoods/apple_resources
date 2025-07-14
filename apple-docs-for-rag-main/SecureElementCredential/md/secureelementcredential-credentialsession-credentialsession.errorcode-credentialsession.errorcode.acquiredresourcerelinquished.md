

- SecureElementCredential
- CredentialSession
- CredentialSession.ErrorCode
-  CredentialSession.ErrorCode.acquiredResourceRelinquished 

Case

# CredentialSession.ErrorCode.acquiredResourceRelinquished

The system relinquished an underlying shared resource, preventing the operation from completing.

iOS 18.1+iPadOS 18.1+

``` source
case acquiredResourceRelinquished
```

## Discussion

When the system throws this error, it also reverts the session state to CredentialSession.State.management.

You can attempt your operation again after receiving this error.

## See Also

### Temporary error codes

case resourceUnavailable

The requested resource is unavailable.

