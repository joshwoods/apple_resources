

- UIKit
- UIFont
-  systemFont(ofSize:weight:width:) 

Type Method

# systemFont(ofSize:weight:width:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class func systemFont(
    ofSize fontSize: CGFloat,
    weight: UIFont.Weight,
    width: UIFont.Width
) -> UIFont
```

## See Also

### Creating System Fonts

class func systemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in the specified size.

class func systemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the font object for standard interface items in the specified size and weight.

struct Weight

Constants that represent standard typeface styles.

struct Width

class func boldSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in boldface type in the specified size.

class func italicSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in italic type in the specified size.

class func monospacedSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the fixed-width font for standard interface text in the specified size.

class func monospacedDigitSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the standard system font with all digits of consistent width.

