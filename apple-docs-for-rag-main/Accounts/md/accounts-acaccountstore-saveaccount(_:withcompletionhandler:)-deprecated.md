

- Accounts
- ACAccountStore
-  saveAccount(\_:withCompletionHandler:) Deprecated

Instance Method

# saveAccount(\_:withCompletionHandler:)

Saves an account to the Accounts database.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
func saveAccount(
    _ account: ACAccount!,
    withCompletionHandler completionHandler: ACAccountStoreSaveCompletionHandler!
)
```

``` source
func saveAccount(_ account: ACAccount!) async throws -> Bool
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Parameters 

`account`  

The account to save.

`completionHandler`  

The handler to call when the operation completes. The handler is called on an arbitrary queue.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func saveAccount(_ account: ACAccount!) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

If the account type supports authentication and the account isn’t authenticated, the account server uses the account’s credentials to authenticate it. If the authentication is successful, the account is saved; otherwise it’s not saved.

## See Also

### Saving Accounts

typealias ACAccountStoreSaveCompletionHandler

Specifies a handler to call when an Accounts database operation is complete.

