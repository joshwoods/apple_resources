

- Accounts
- ACAccountStore
-  requestAccessToAccounts(with:options:completion:) Deprecated

Instance Method

# requestAccessToAccounts(with:options:completion:)

Obtains permission to access protected user properties.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
func requestAccessToAccounts(
    with accountType: ACAccountType!,
    options: [AnyHashable : Any]! = [:],
    completion: ACAccountStoreRequestAccessCompletionHandler!
)
```

``` source
func requestAccessToAccounts(
    with accountType: ACAccountType!,
    options: [AnyHashable : Any]! = [:]
) async throws -> Bool
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Parameters 

`accountType`  

The account type.

`options`  

A dictionary of options, if options are required by the account type; otherwise, `nil`.

`completion`  

The handler to call when the request has completed. The handler is called on an arbitrary queue.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func requestAccessToAccounts(with accountType: ACAccountType!, options: [AnyHashable : Any]! = [:]) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Certain account types (such as Facebook) require an options dictionary. This method throws an `NSInvalidArgumentException` if the options dictionary isn’t provided for such account types. Conversely, if the account type doesn’t require an options dictionary, the `options` parameter must be `nil`.

## See Also

### Requesting Access

typealias ACAccountStoreRequestAccessCompletionHandler

Specifies a handler to call when access is granted or denied.

