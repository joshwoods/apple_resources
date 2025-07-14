

- UIKit
-  NSTextAlignment 

Enumeration

# NSTextAlignment

Constants that specify text alignment.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum NSTextAlignment
```

## Topics

### Constants

case left

Text is left-aligned.

case right

Text is right-aligned.

case center

Text is center-aligned.

case justified

Text is justified.

case natural

Text uses the default alignment for the current localization of the app.

### Initializers

init(CTTextAlignment)

Converts a Core Text alignment constant value to the matching constant value in UIKit.

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

