

- Security
- SecItemImportExportKeyParameters
-  alertTitle 

Instance Property

# alertTitle

The title to display in the secure passphrase alert panel.

macOS 10.0+

``` source
var alertTitle: Unmanaged?
```

## Discussion

When importing or exporting a key, if you set the securePassphrase flag bit, you can optionally use this field to specify a string for the password panel’s title bar.

