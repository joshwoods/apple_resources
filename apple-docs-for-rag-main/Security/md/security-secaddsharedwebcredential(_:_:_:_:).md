

- Security
-  SecAddSharedWebCredential(\_:\_:\_:\_:) 

Function

# SecAddSharedWebCredential(\_:\_:\_:\_:)

Asynchronously stores (or updates) a shared password for a website.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func SecAddSharedWebCredential(
    _ fqdn: CFString,
    _ account: CFString,
    _ password: CFString?,
    _ completionHandler: @escaping (CFError?) -> Void
)
```

## Parameters 

`fqdn`  

The fully qualified domain name of the website requiring the password.

`account`  

The account name associated with this password.

`password`  

The password to be stored. Pass `NULL` to remove a shared password if it exists.

`completionHandler`  

A block invoked when the function has completed.

The block takes one argument:

`error`  
If the shared password was successfully added (or removed), `NULL`; if not successful, a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 object that encapsulates the reason why the password could not be added (or removed). The error reference is automatically released after this handler is called, though you may optionally retain it for as long as needed.

## Mentioned in 

Managing Shared Credentials

## Discussion

This function adds a shared password item that will be accessible by Safari and apps that have the specified fully qualified domain name in their Associated Domains Entitlement. If a shared password item already exists for the specified website and account, it is updated with the provided password. To remove a password, pass `NULL` for the password parameter.

Note

Because a request involving shared web credentials may potentially require user interaction or other verification to be approved, this function is dispatched asynchronously; your code provides a completion handler that is called as soon as the results (if any) are available.

When this function is called, the system tries to get the site association file from the server. If the file is unavailable, the sever returns a 500-599 code.

