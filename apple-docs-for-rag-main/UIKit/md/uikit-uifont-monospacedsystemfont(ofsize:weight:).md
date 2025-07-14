

- UIKit
- UIFont
-  monospacedSystemFont(ofSize:weight:) 

Type Method

# monospacedSystemFont(ofSize:weight:)

Returns the fixed-width font for standard interface text in the specified size.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func monospacedSystemFont(
    ofSize fontSize: CGFloat,
    weight: UIFont.Weight
) -> UIFont
```

## Parameters 

`fontSize`  

The size (in points) for the font. This value must be greater than `0.0`.

`weight`  

The weight of the font, specified as a font weight constant. For a list of possible values, see UIFont.Weight. Avoid passing an arbitrary floating-point number for `weight`, because a font might not include a variant for every weight.

## Return Value

A font object of the specified size.

## Discussion

This method provides the same font as the monospaced system font descriptor. For design guidance, see Typography in the Human Interface Guidelines.

Note

To display text in the standard system font, but with fixed-width digits, use monospacedDigitSystemFont(ofSize:weight:) instead.

## See Also

### Creating System Fonts

class func systemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in the specified size.

class func systemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the font object for standard interface items in the specified size and weight.

struct Weight

Constants that represent standard typeface styles.

class func systemFont(ofSize: CGFloat, weight: UIFont.Weight, width: UIFont.Width) -> UIFont

struct Width

class func boldSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in boldface type in the specified size.

class func italicSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in italic type in the specified size.

class func monospacedDigitSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the standard system font with all digits of consistent width.

