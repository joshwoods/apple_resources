

- Security
- SecItemImportExportKeyParameters
-  keyAttributes 

Instance Property

# keyAttributes

An array containing zero or more key attributes for an imported key.

macOS 10.0+

``` source
var keyAttributes: Unmanaged?
```

## Discussion

Valid values are kSecAttrIsPermanent, kSecAttrIsSensitive, and kSecAttrIsExtractable. If you set this attribute array to `NULL`, the following defaults are used:

- The item is marked permanent if a keychain is specified.

- The item is marked sensitive if it is a private key.

- The item is marked extractable by default.

