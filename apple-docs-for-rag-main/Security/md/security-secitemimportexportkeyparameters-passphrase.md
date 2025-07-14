

- Security
- SecItemImportExportKeyParameters
-  passphrase 

Instance Property

# passphrase

The password to use during key import or export.

macOS 10.0+

``` source
var passphrase: Unmanaged?
```

## Discussion

You may specify either a CFString or a CFData instance for the passphrase. The PKCS12 format requires passwords in Unicode format, and passing in a CFString as the password is the surest way to meet this requirement (and ensure compatibility with other implementations). If you supply a CFData instance as the password for a PKCS12 export operation, the data is assumed to be in UTF8 form and converted as appropriate.

When importing or exporting keys (SecKey objects) in one of the wrapped formats (SecExternalFormat.formatWrappedOpenSSL, SecExternalFormat.formatWrappedSSH, or SecExternalFormat.formatWrappedPKCS8) or in PKCS12 format, you must either explicitly specify the passphrase field or set the securePassphrase bit the flags field (to prompt the user to enter the password).

