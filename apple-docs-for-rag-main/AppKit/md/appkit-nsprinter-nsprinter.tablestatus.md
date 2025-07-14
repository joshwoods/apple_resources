

- AppKit
- NSPrinter
-  NSPrinter.TableStatus 

Enumeration

# NSPrinter.TableStatus

Constants that describe the state of a printer information table stored by a printer object.

macOS

``` source
enum TableStatus
```

## Overview

These constants are used by statusForTable:.

## Topics

### Constants

case ok

Printer table was found and is valid.

case notFound

Printer table was not found.

case error

Printer table is not valid.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

