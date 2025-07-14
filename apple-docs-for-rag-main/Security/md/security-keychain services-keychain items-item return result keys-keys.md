

- Security
- Keychain services
- Keychain items
-  Item return result keys 

API Collection

# Item return result keys

Specify how you want returned keychain item data formatted.

## Overview

When you use one of the SecItemAdd(_:_:) or SecItemCopyMatching(_:_:) functions to add or search for keychain items, these functions return the item’s data and attributes through the `result` parameter to which you provide a pointer. Use the item result keys described below in the corresponding query dictionary to indicate how those results should be formatted:

- If you request a data reference with kSecReturnRef, the search returns a reference of type SecKeychainItem, SecKey, SecCertificate, SecIdentity, or doc://com.apple.documentation/documentation/corefoundation/cfdata-rv9, depending on the class of the item.

- If you request a persistent data reference using kSecReturnPersistentRef, the search returns an item reference of type doc://com.apple.documentation/documentation/corefoundation/cfdata-rv9 that you can store on disk or pass between processes. You later convert persistent references to regular references with another call to the SecItemCopyMatching(_:_:) function, using an array of persistent references (of the same item class) as the value for the kSecMatchItemList key.

- If you ask for the data itself with kSecReturnData, the search returns a doc://com.apple.documentation/documentation/corefoundation/cfdata-rv9 instance that holds the actual data. This is typically what you want for password items. To undo the encryption it added prior to storing the item, keychain services decrypts the data before returning it to you. Don’t use kSecReturnData for cryptographic key or identity items, as the key material may not be extractable. Instead, call SecKeyCopyExternalRepresentation(_:_:), and check the `error` parameter if it returns `nil`.

- If you request the item’s attributes using kSecReturnAttributes or more than one return type, the search returns a dictionary. Item attributes are represented directly as key-value pairs in this dictionary, while the item’s data appears in one or more of the previously mentioned forms, and is associated with the appropriate item value type key from Item return result keys.

- When you specify a match limit greater than one, the search produces an array. Each element of the array is itself a search result formatted according to the previous rules.

## Topics

### Item result keys

Keys you use to specify the type of results to return from a keychain item search or add operation.

let kSecReturnData: CFString

A key whose value is a Boolean that indicates whether or not to return item data.

let kSecReturnAttributes: CFString

A key whose value is a Boolean indicating whether or not to return item attributes.

let kSecReturnRef: CFString

A key whose value is a Boolean indicating whether or not to return a reference to an item.

let kSecReturnPersistentRef: CFString

A key whose value is a Boolean indicating whether or not to return a persistent reference to an item.

### Item value type keys

Keys that appear in the result dictionary when you specify more than one search result key.

let kSecValueData: CFString

A key whose value is the item’s data.

let kSecValueRef: CFString

A key whose value is a reference to the item.

let kSecValuePersistentRef: CFString

A key whose value is a persistent reference to the item.

