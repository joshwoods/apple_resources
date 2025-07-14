

- UIKit
-  NSWritingDirection 

Enumeration

# NSWritingDirection

Constants that specify the writing direction.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum NSWritingDirection
```

## Topics

### Constants

case natural

The writing direction of the current script that the system determines using the Unicode Bidi Algorithm rules P2 and P3.

case leftToRight

The writing direction is left to right.

case rightToLeft

The writing direction is right to left.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining writing direction

class func defaultWritingDirection(forLanguage: String?) -> NSWritingDirection

Returns the default writing direction for the specified language.

var baseWritingDirection: NSWritingDirection

The base writing direction for the paragraph.

