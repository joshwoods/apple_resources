

- UIKit
- UIFont
-  monospacedDigitSystemFont(ofSize:weight:) 

Type Method

# monospacedDigitSystemFont(ofSize:weight:)

Returns the standard system font with all digits of consistent width.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func monospacedDigitSystemFont(
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

A font object of the specified size and weight, with variable-width text and fixed-width digits.

## Discussion

The system font uses proportional spacing. When displaying numerical data, you can use this method to retrieve a monospace font for displaying that data. With a monospaced font, each digit occupies the same amount of space, which makes it easier to read numbers that are stacked vertically.

Note

This method returns the same font as systemFont(ofSize:weight:), but with modified digits. If you want all characters to be fixed-width, use monospacedSystemFont(ofSize:weight:) instead.

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

class func monospacedSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the fixed-width font for standard interface text in the specified size.

