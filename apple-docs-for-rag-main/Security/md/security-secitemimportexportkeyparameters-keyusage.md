

- Security
- SecItemImportExportKeyParameters
-  keyUsage 

Instance Property

# keyUsage

An array containing usage attributes applied to a key on import.

macOS 10.0+

``` source
var keyUsage: Unmanaged?
```

## Discussion

The array may contain any of the following key usage constants:

- kSecAttrCanEncrypt

- kSecAttrCanDecrypt

- kSecAttrCanDerive

- kSecAttrCanSign

- kSecAttrCanVerify

- kSecAttrCanWrap

- kSecAttrCanUnwrap

If the array is `NULL`, all operations are allowed by default.

