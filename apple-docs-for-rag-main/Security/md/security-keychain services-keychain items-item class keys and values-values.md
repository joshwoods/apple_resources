

- Security
- Keychain services
- Keychain items
-  Item class keys and values 

API Collection

# Item class keys and values

Specify the class of a keychain item.

## Overview

Keychain items come in a variety of classes according to the kind of data they hold, such as passwords, cryptographic keys, and certificates. The item’s class dictates which attributes apply and enables the system to decide whether to encrypt the data. For example, the system encrypts passwords, but not certificates because they aren’t secret.

Use the key and one of the corresponding values listed here to specify the class for a new item you create with a call to the SecItemAdd(_:_:) function by placing the key/value pair in the `attributes` dictionary.

Later, use this same pair in the `query` dictionary when searching for an item with one of the SecItemCopyMatching(_:_:), SecItemUpdate(_:_:), or SecItemDelete(_:) functions.

## Topics

### Item class keys

let kSecClass: CFString

A dictionary key whose value is the item’s class.

### Item class values

Values you use with the kSecClass key.

let kSecClassGenericPassword: CFString

The value that indicates a generic password item.

let kSecClassInternetPassword: CFString

The value that indicates an Internet password item.

let kSecClassCertificate: CFString

The value that indicates a certificate item.

let kSecClassKey: CFString

The value that indicates a cryptographic key item.

let kSecClassIdentity: CFString

The value that indicates an identity item.

