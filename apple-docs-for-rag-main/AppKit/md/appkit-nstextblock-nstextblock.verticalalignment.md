

- AppKit
- NSTextBlock
-  NSTextBlock.VerticalAlignment 

Enumeration

# NSTextBlock.VerticalAlignment

The following constants specify values used by the property verticalAlignment to specify vertical alignment.

macOS

``` source
enum VerticalAlignment
```

## Topics

### Constants

case topAlignment

Aligns adjacent blocks at their top.

case middleAlignment

Aligns adjacent blocks at their middle.

case bottomAlignment

Aligns adjacent blocks at their bottom.

case baselineAlignment

Aligns adjacent blocks at the baseline of the first line of text in the block.

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

### Getting and setting alignment

var verticalAlignment: NSTextBlock.VerticalAlignment

The vertical alignment of the text block.

