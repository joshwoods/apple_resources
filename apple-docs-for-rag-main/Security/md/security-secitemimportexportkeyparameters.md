

- Security
-  SecItemImportExportKeyParameters 

Structure

# SecItemImportExportKeyParameters

The import/export parameter structure.

macOS 10.0+

``` source
struct SecItemImportExportKeyParameters
```

## Overview

Use this structure as the `keyParams` input parameter to the SecItemExport(_:_:_:_:_:) and the SecItemImport(_:_:_:_:_:_:_:_:) functions.

## Topics

### Instance Properties

var accessRef: Unmanaged&lt;SecAccess>?

Specifies the initial access controls of imported private keys.

var alertPrompt: Unmanaged&lt;CFString>?

The prompt to display in the secure passphrase alert panel.

var alertTitle: Unmanaged&lt;CFString>?

The title to display in the secure passphrase alert panel.

var flags: SecKeyImportExportFlags

The bitwise `OR` of zero or more key import/export flags.

var keyAttributes: Unmanaged&lt;CFArray>?

An array containing zero or more key attributes for an imported key.

var keyUsage: Unmanaged&lt;CFArray>?

An array containing usage attributes applied to a key on import.

var passphrase: Unmanaged&lt;CFTypeRef>?

The password to use during key import or export.

var version: UInt32

The version of this structure.

### Initializers

init()

init(version: UInt32, flags: SecKeyImportExportFlags, passphrase: Unmanaged&lt;CFTypeRef>?, alertTitle: Unmanaged&lt;CFString>?, alertPrompt: Unmanaged&lt;CFString>?, accessRef: Unmanaged&lt;SecAccess>?, keyUsage: Unmanaged&lt;CFArray>?, keyAttributes: Unmanaged&lt;CFArray>?)

## Relationships

### Conforms To

- BitwiseCopyable

