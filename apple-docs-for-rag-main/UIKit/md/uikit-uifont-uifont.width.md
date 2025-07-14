

- UIKit
- UIFont
-  UIFont.Width 

Structure

# UIFont.Width

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 9.0+

``` source
struct Width
```

## Topics

### Font widths

static let compressed: UIFont.Width

static let condensed: UIFont.Width

static let expanded: UIFont.Width

static let standard: UIFont.Width

### Initializers

init(CGFloat)

init(rawValue: CGFloat)

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating System Fonts

class func systemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in the specified size.

class func systemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the font object for standard interface items in the specified size and weight.

struct Weight

Constants that represent standard typeface styles.

class func systemFont(ofSize: CGFloat, weight: UIFont.Weight, width: UIFont.Width) -> UIFont

class func boldSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in boldface type in the specified size.

class func italicSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in italic type in the specified size.

class func monospacedSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the fixed-width font for standard interface text in the specified size.

class func monospacedDigitSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the standard system font with all digits of consistent width.

