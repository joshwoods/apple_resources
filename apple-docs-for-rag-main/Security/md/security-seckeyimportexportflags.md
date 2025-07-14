

- Security
-  SecKeyImportExportFlags 

Structure

# SecKeyImportExportFlags

The import/export parameter structure flags.

macOS 10.0+

``` source
struct SecKeyImportExportFlags
```

## Overview

Use an instance of this structure to set the flags property in the SecItemImportExportKeyParameters import/export structure.

## Topics

### Initializers

init(rawValue: UInt32)

Initialize a key import/export flag structure.

### Constants

static var importOnlyOne: SecKeyImportExportFlags

A flag that you set to prevent importing more than one private key.

static var securePassphrase: SecKeyImportExportFlags

A flag that indicates the user should be prompted for a passphrase on import or export.

static var noAccessControl: SecKeyImportExportFlags

A flag that indicates imported private keys have no access object attached to them.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

