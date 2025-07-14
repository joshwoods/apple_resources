

- Security
-  SecKeyImportExportParameters Deprecated

Structure

# SecKeyImportExportParameters

The legacy import/export parameter structure.

macOS 10.0+

``` source
struct SecKeyImportExportParameters
```

Deprecated

This structure is passed in the `keyParams` parameter as input to the deprecated SecKeychainItemExport and SecKeychainItemImport functions. Use SecItemExport(_:_:_:_:_:) and SecItemImport(_:_:_:_:_:_:_:_:) instead. The newer functions rely on the similar but distinct SecItemImportExportKeyParameters structure as input rather than the structure defined here.

## Overview

PKCS12 is an abbreviation for Public-Key Cryptography Standard \# 12. This standard, by RSA Security, provides a format for external representation of keys and certificates and is described in *PKCS 12 v1.0: Personal Information Exchange Syntax*.

## Topics

### Instance Properties

var accessRef: Unmanaged&lt;SecAccess>?

Specifies the initial access controls of imported private keys.

var alertPrompt: Unmanaged&lt;CFString>

The prompt to display in the secure passphrase alert panel.

var alertTitle: Unmanaged&lt;CFString>

The title to display in the secure passphrase alert panel.

var flags: SecKeyImportExportFlags

The bitwise `OR` of zero or more key import/export flags.

var keyAttributes: CSSM_KEYATTR_FLAGS

A word of bits constituting the low-level attribute flags for imported keys.

var keyUsage: CSSM_KEYUSE

A word of bits constituting the low-level use flags for imported keys.

var passphrase: Unmanaged&lt;CFTypeRef>?

The password to use during key import or export.

var version: UInt32

The version of this structure.

### Initializers

init(version: UInt32, flags: SecKeyImportExportFlags, passphrase: Unmanaged&lt;CFTypeRef>?, alertTitle: Unmanaged&lt;CFString>, alertPrompt: Unmanaged&lt;CFString>, accessRef: Unmanaged&lt;SecAccess>?, keyUsage: CSSM_KEYUSE, keyAttributes: CSSM_KEYATTR_FLAGS)

Creates a new import/export parameter structure.

## Relationships

### Conforms To

- BitwiseCopyable

