

- Accounts
-  ACAccountStoreRemoveCompletionHandler 

Type Alias

# ACAccountStoreRemoveCompletionHandler

Specifies a handler to call when an account is removed from the store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.8+

``` source
typealias ACAccountStoreRemoveCompletionHandler = (Bool, (any Error)?) -> Void
```

## Discussion

The completion handler parameters are:

`success`  
A Boolean value indicating whether the operation was successful. true if successful, otherwise false.

`error`  
An error, if one occurred.

## See Also

### Removing Accounts

func removeAccount(ACAccount!, withCompletionHandler: ACAccountStoreRemoveCompletionHandler!)

Removes an account from the account store.

Deprecated

