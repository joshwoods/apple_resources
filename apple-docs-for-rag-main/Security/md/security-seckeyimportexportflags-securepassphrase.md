

- Security
- SecKeyImportExportFlags
-  securePassphrase 

Type Property

# securePassphrase

A flag that indicates the user should be prompted for a passphrase on import or export.

macOS 10.0+

``` source
static var securePassphrase: SecKeyImportExportFlags { get }
```

## Discussion

When set, the password for import or export is obtained by user prompt. (A password is sometimes referred to as a passphrase to emphasize the fact that a longer string that includes non-letter characters, such as numbers, punctuation, and spaces, is more secure than a simple word.) Otherwise, you must provide the password in the passphrase field of the SecItemImportExportKeyParameters structure. A user-supplied password is preferred, because it avoids having the cleartext password appear in the application’s address space at any time.

