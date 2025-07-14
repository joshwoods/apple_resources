

- Authentication Services
- ASCredentialIdentityStoreError
-  storeBusy 

Type Property

# storeBusy

The operation failed because the credential identity store is busy.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static var storeBusy: ASCredentialIdentityStoreError.Code { get }
```

## Discussion

Attempt the operation again at a later time.

## See Also

### Error domain

let ASCredentialIdentityStoreErrorDomain: String

The domain for a credential identity store error.

static var internalError: ASCredentialIdentityStoreError.Code

The operation failed due to an internal error.

static var storeDisabled: ASCredentialIdentityStoreError.Code

The operation failed because the credential identity store is disabled.

enum Code

Constants that represent credential identity store error codes.

