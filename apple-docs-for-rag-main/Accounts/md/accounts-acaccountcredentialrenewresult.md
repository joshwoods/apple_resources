

- Accounts
-  ACAccountCredentialRenewResult 

Enumeration

# ACAccountCredentialRenewResult

Status codes of credential renewal requests.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.8+

``` source
enum ACAccountCredentialRenewResult
```

## Topics

### Constants

case renewed

The account’s credentials have been renewed and are now associated with the account.

case rejected

Renewal failed because the user revoked your access to their account.

case failed

A non-user-initiated cancel of the prompt.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Renewing Account Credentials

func renewCredentials(for: ACAccount!, completion: ACAccountStoreCredentialRenewalHandler!)

Renews account credentials when the credentials are no longer valid.

Deprecated

typealias ACAccountStoreCredentialRenewalHandler

Specifies a handler to call when credentials are renewed.

