

- Security
- SecItemImportExportKeyParameters
-  init(version:flags:passphrase:alertTitle:alertPrompt:accessRef:keyUsage:keyAttributes:) 

Initializer

# init(version:flags:passphrase:alertTitle:alertPrompt:accessRef:keyUsage:keyAttributes:)

macOS 10.0+

``` source
init(
    version: UInt32,
    flags: SecKeyImportExportFlags,
    passphrase: Unmanaged?,
    alertTitle: Unmanaged?,
    alertPrompt: Unmanaged?,
    accessRef: Unmanaged?,
    keyUsage: Unmanaged?,
    keyAttributes: Unmanaged?
)
```

