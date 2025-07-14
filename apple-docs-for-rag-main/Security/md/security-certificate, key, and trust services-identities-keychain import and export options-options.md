

- Security
- Certificate, Key, and Trust Services
- Identities
-  Keychain Import and Export Options 

API Collection

# Keychain Import and Export Options

Use these constants when you pass dictionary-based arguments to import and export functions.

## Topics

### Constants

let kSecImportExportPassphrase: CFString

A passphrase (represented by a `CFStringRef` object) to be used when exporting to or importing from PKCS#12 format.

let kSecImportExportKeychain: CFString

A keychain represented by a SecKeychainRef to be used as the target when importing or exporting.

let kSecImportExportAccess: CFString

An initial access control list represented by a SecAccess object.

