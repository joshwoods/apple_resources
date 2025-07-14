

- AppKit
-  NSFocusRingType 

Enumeration

# NSFocusRingType

Constants that describe the style of the focus ring.

macOS

``` source
enum NSFocusRingType
```

## Overview

The focus ring type is used by NSView and NSCell to configure whether and how a control draws its focus ring.

## Topics

### Constants

case `default`

The default focus ring type for a view or cell.

case none

No focus ring.

case exterior

The standard Aqua focus ring.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Drawing Focus Rings

func set()

Specifies how the system draws the focus ring.

enum NSFocusRingPlacement

Constants that indicate how the system draws the focus ring.

