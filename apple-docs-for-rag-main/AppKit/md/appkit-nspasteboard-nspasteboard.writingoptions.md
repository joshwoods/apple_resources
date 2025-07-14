

- AppKit
- NSPasteboard
-  NSPasteboard.WritingOptions 

Structure

# NSPasteboard.WritingOptions

Type to specify options for writing to a pasteboard.

macOS 10.6+

``` source
struct WritingOptions
```

## Overview

For possible values, see Pasteboard Writing Options.

## Topics

### Options

static var promised: NSPasteboard.WritingOptions

Data for a type with this option is promised, not immediately written.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

