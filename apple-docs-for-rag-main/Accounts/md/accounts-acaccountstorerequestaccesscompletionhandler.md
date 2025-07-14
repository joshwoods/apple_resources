

- Accounts
-  ACAccountStoreRequestAccessCompletionHandler 

Type Alias

# ACAccountStoreRequestAccessCompletionHandler

Specifies a handler to call when access is granted or denied.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.8+

``` source
typealias ACAccountStoreRequestAccessCompletionHandler = (Bool, (any Error)?) -> Void
```

## Discussion

The completion handler parameters are:

`granted`  
A Boolean value indicating whether access is granted. true if access is granted; otherwise false.

`error`  
An error, if one occurred.

## See Also

### Requesting Access

func requestAccessToAccounts(with: ACAccountType!, options: [AnyHashable : Any]!, completion: ACAccountStoreRequestAccessCompletionHandler!)

Obtains permission to access protected user properties.

Deprecated

