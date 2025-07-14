

- Security
- SecKeyImportExportFlags
-  importOnlyOne 

Type Property

# importOnlyOne

A flag that you set to prevent importing more than one private key.

macOS 10.0+

``` source
static var importOnlyOne: SecKeyImportExportFlags { get }
```

## Discussion

Prevents the importing of more than one private key by the SecKeychainItemImport function. If the `importKeychain` parameter is `NULL`, this bit is ignored. Otherwise, if this bit is set and there is more than one key in the incoming external representation, no items are imported to the specified keychain and the error `errSecMultipleKeys` is returned.

