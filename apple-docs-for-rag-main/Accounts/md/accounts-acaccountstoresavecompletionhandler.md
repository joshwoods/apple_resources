

- Accounts
-  ACAccountStoreSaveCompletionHandler 

Type Alias

# ACAccountStoreSaveCompletionHandler

Specifies a handler to call when an Accounts database operation is complete.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.8+

``` source
typealias ACAccountStoreSaveCompletionHandler = (Bool, (any Error)?) -> Void
```

## Discussion

The completion handler parameters are:

`success`  
A Boolean value indicating whether the operation is successful. true if the operation is successful; otherwise false.

`error`  
An error, if one occurred.

## See Also

### Saving Accounts

func saveAccount(ACAccount!, withCompletionHandler: ACAccountStoreSaveCompletionHandler!)

Saves an account to the Accounts database.

Deprecated

