

- Accounts
- ACAccountStore
-  renewCredentials(for:completion:) Deprecated

Instance Method

# renewCredentials(for:completion:)

Renews account credentials when the credentials are no longer valid.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
func renewCredentials(
    for account: ACAccount!,
    completion completionHandler: ACAccountStoreCredentialRenewalHandler!
)
```

``` source
func renewCredentials(for account: ACAccount!) async throws -> ACAccountCredentialRenewResult
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Parameters 

`account`  

The account to renew credentials.

`completionHandler`  

The handler to call when the renewal has completed.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func renewCredentials(for account: ACAccount!) async throws -> ACAccountCredentialRenewResult
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

For Twitter and Sina Weibo accounts, this method prompts the user to go to Settings to re-enter their password.

For Facebook accounts, if the access token has become invalid due to a regular expiration, this method obtains a new one.

If the user has deauthorized your app, this renewal request returns `ACAccountCredentialRenewResultRejected`.

## See Also

### Renewing Account Credentials

typealias ACAccountStoreCredentialRenewalHandler

Specifies a handler to call when credentials are renewed.

enum ACAccountCredentialRenewResult

Status codes of credential renewal requests.

