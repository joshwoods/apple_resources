

- Accounts
- ACAccountStore
-  removeAccount(\_:withCompletionHandler:) Deprecated

Instance Method

# removeAccount(\_:withCompletionHandler:)

Removes an account from the account store.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
func removeAccount(
    _ account: ACAccount!,
    withCompletionHandler completionHandler: ACAccountStoreRemoveCompletionHandler!
)
```

``` source
func removeAccount(_ account: ACAccount!) async throws -> Bool
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Parameters 

`account`  

The account to remove.

`completionHandler`  

The handler to call when the removal has completed.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This call will fail if you don’t have sufficient rights to remove the account.

## See Also

### Removing Accounts

typealias ACAccountStoreRemoveCompletionHandler

Specifies a handler to call when an account is removed from the store.

