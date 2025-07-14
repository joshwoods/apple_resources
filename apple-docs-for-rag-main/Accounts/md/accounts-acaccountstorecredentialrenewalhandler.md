

- Accounts
-  ACAccountStoreCredentialRenewalHandler 

Type Alias

# ACAccountStoreCredentialRenewalHandler

Specifies a handler to call when credentials are renewed.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.8+

``` source
typealias ACAccountStoreCredentialRenewalHandler = (ACAccountCredentialRenewResult, (any Error)?) -> Void
```

## Discussion

The renewal handler parameters are:

`renewResult`  
The result of the renewal request.

`error`  
An error, if one occurred.

## See Also

### Renewing Account Credentials

func renewCredentials(for: ACAccount!, completion: ACAccountStoreCredentialRenewalHandler!)

Renews account credentials when the credentials are no longer valid.

Deprecated

enum ACAccountCredentialRenewResult

Status codes of credential renewal requests.

