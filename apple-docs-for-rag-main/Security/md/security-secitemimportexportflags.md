

- Security
-  SecItemImportExportFlags 

Structure

# SecItemImportExportFlags

The import and export function flags.

macOS 10.0+

``` source
struct SecItemImportExportFlags
```

## Overview

Use an instance of this structure a the flags input to the SecItemImport(_:_:_:_:_:_:_:_:) and SecItemExport(_:_:_:_:_:) functions.

## Topics

### Initializers

init(rawValue: UInt32)

Initialize an item import/export flag structure.

### Constants

static var pemArmour: SecItemImportExportFlags

A flag that indicates the exported data should have PEM armor.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

