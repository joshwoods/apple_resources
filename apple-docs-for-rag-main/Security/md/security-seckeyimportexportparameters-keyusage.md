

- Security
- SecKeyImportExportParameters
-  keyUsage 

Instance Property

# keyUsage

A word of bits constituting the low-level use flags for imported keys.

macOS 10.0+

``` source
var keyUsage: CSSM_KEYUSE
```

## Discussion

Use flags defined in `cssmtype.h`. If this field is `0` or `keyParams` is `NULL`, the default value is `CSSM_KEYUSE_ANY`.

