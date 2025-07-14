

- Core Text
-  CTTextAlignment 

Enumeration

# CTTextAlignment

Constants that specify text alignment.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTTextAlignment
```

## Topics

### Constants

case left

Text is visually left-aligned.

case right

Text is visually right-aligned.

case center

Text is visually center-aligned.

case justified

Text is fully justified.

case natural

Text uses the natural alignment of the text’s script.

### Initializers

init(NSTextAlignment)

Converts a UIKit text alignment constant value to the matching constant value that Core Text uses.

init?(rawValue: UInt8)

### Deprecated

static var kCTLeftTextAlignment: CTTextAlignment

Text is visually left-aligned.

Deprecated

static var kCTRightTextAlignment: CTTextAlignment

Text is visually right-aligned.

Deprecated

static var kCTCenterTextAlignment: CTTextAlignment

Text is visually center-aligned.

Deprecated

static var kCTJustifiedTextAlignment: CTTextAlignment

Text is fully justified.

Deprecated

static var kCTNaturalTextAlignment: CTTextAlignment

Text uses the natural alignment of the text’s script.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum CTLineBreakMode

These constants specify what happens when a line is too long for its frame.

enum CTWritingDirection

These constants specify the writing direction.

enum CTParagraphStyleSpecifier

Constants used to query and modify a paragraph style object.

