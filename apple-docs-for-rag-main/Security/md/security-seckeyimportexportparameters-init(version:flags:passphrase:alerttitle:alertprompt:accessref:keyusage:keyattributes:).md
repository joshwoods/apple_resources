

- Security
- SecKeyImportExportParameters
-  init(version:flags:passphrase:alertTitle:alertPrompt:accessRef:keyUsage:keyAttributes:) 

Initializer

# init(version:flags:passphrase:alertTitle:alertPrompt:accessRef:keyUsage:keyAttributes:)

Creates a new import/export parameter structure.

macOS 10.0+

``` source
init(
    version: UInt32,
    flags: SecKeyImportExportFlags,
    passphrase: Unmanaged?,
    alertTitle: Unmanaged,
    alertPrompt: Unmanaged,
    accessRef: Unmanaged?,
    keyUsage: CSSM_KEYUSE,
    keyAttributes: CSSM_KEYATTR_FLAGS
)
```

