

- Security
-  kSecMatchItemList 

Global Variable

# kSecMatchItemList

A key whose value indicates a list of items to search.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecMatchItemList: CFString
```

## Mentioned in 

Updating and deleting keychain items

## Discussion

To provide your own set of items to be filtered by a search query rather than searching the keychain, specify this search key in a call to the SecItemCopyMatching(_:_:) function with a value that consists of an object of type CFArray where the array contains either SecKeychainItem, SecKey, SecCertificate, SecIdentity, or CFData items. The objects in the provided array must all be of the same type.

To convert from persistent item references to normal item references, specify this search key in a call to the SecItemCopyMatching(_:_:) function with a value of type CFArray where the array contains one or more CFData elements (the persistent references), and a return-type key of kSecReturnRef whose value is kCFBooleanTrue.

To delete an item identified by a transient reference, specify the kSecMatchItemList search key in a call to the SecItemDelete(_:) function with a reference returned by using the kSecReturnRef return type key in a previous call to the SecItemCopyMatching(_:_:) or SecItemAdd(_:_:) functions.

To delete an item identified by a persistent reference, specify the kSecMatchItemList search key in a call to the SecItemDelete(_:) function with a persistent reference returned by using the kSecReturnPersistentRef return type key to the SecItemCopyMatching(_:_:) or SecItemAdd(_:_:) functions.

