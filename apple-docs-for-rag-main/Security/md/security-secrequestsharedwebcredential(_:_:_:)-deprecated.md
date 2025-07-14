

- Security
-  SecRequestSharedWebCredential(\_:\_:\_:) Deprecated

Function

# SecRequestSharedWebCredential(\_:\_:\_:)

Asynchronously obtains one or more shared passwords for a website.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 11.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func SecRequestSharedWebCredential(
    _ fqdn: CFString?,
    _ account: CFString?,
    _ completionHandler: @escaping (CFArray?, CFError?) -> Void
)
```

Deprecated

Use ASAuthorizationController to make an ASAuthorizationPasswordRequest instead.

## Parameters 

`fqdn`  

(Optional) The fully qualified domain name of the website for which passwords are being requested. If `NULL` is passed in this argument, the domain name(s) listed in the calling app’s Associated Domains Entitlement are searched implicitly.

`account`  

(Optional) The account name for which passwords are being requested. The account may be `NULL` to request all of the shared credentials that are available for the site, allowing the caller to discover an existing account.

`completionHandler`  

A block that is called to deliver the requested credentials.

The block takes two arguments:

`credentials`  
An array containing the requested passwords. If no matching items are found, the credentials array is empty. The credentials reference is automatically released after this handler is called, though you may optionally retain it for as long as needed.

`error`  
If the shared password was successfully added (or removed), `NULL`; if not successful, a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 object that encapsulates the reason why the password could not be added (or removed). The error reference is automatically released after this handler is called, though you may optionally retain it for as long as needed.

## Mentioned in 

Managing Shared Credentials

## Discussion

This function requests one or more shared passwords for a given website, depending on whether the optional account parameter is supplied. To obtain results, the website specified in the `fqdn` parameter must be one that matches an entry in the calling app’s Associated Domains Entitlement.

If matching shared password items are found, the credentials provided to the completion handler will be a CFArray data type containing CFDictionary entries. Each dictionary contains the following pairs:

| Key | Value |
|----|----|
| kSecAttrServer | CFString (the website) |
| kSecAttrAccount | CFString (the account) |
| kSecSharedPassword | CFString (the password) |

If the found item specifies a nonstandard port number (other than 443 for `https`), the following key may also be present:

| kSecAttrPort | CFNumber (the port number) |
|----|----|

Note

Because a request involving shared web credentials may potentially require user interaction or other verification to be approved, this function is dispatched asynchronously; your code provides a completion handler that will be called as soon as the results (if any) are available.

