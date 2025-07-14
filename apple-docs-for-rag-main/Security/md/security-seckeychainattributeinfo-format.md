

- Security
- SecKeychainAttributeInfo
-  format 

Instance Property

# format

A pointer to the first attribute format in the array.

macOS 10.0+

``` source
var format: UnsafeMutablePointer?
```

## Discussion

Attribute formats are of type `CSSM_DB_ATTRIBUTE_FORMAT` (`CSSM_DB_ATTRIBUTE_FORMAT_STRING`, for example), and are defined in the `cssmtype.h` header.

