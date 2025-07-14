

- Security
- SecKeyImportExportParameters
-  alertPrompt 

Instance Property

# alertPrompt

The prompt to display in the secure passphrase alert panel.

macOS 10.0+

``` source
var alertPrompt: Unmanaged
```

## Discussion

When importing or exporting a key, if you set the securePassphrase flag bit, you can optionally use this field to specify a string for the prompt that appears in the password panel.

