

- AppKit
-  NSFocusRingPlacement 

Enumeration

# NSFocusRingPlacement

Constants that indicate how the system draws the focus ring.

macOS

``` source
enum NSFocusRingPlacement
```

## Topics

### Constants

case above

Draw the focus ring over an image.

case below

Draw the focus ring under text.

case only

Draw the focus ring if you don’t have an image or text.

### Options for Drawing

func set()

Specifies how the system draws the focus ring.

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

enum NSFocusRingType

Constants that describe the style of the focus ring.

