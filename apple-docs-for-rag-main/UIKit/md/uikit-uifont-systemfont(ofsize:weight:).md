

- UIKit
- UIFont
-  systemFont(ofSize:weight:) 

Type Method

# systemFont(ofSize:weight:)

Returns the font object for standard interface items in the specified size and weight.

iOS 8.2+iPadOS 8.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func systemFont(
    ofSize fontSize: CGFloat,
    weight: UIFont.Weight
) -> UIFont
```

## Parameters 

`fontSize`  

The size (in points) to which the font is scaled. This value must be greater than 0.0.

`weight`  

The weight of the font, specified as a font weight constant. For a list of possible values, see “Font Weights” in UIFontDescriptor. Avoid passing an arbitrary floating-point number for `weight`, because a font might not include a variant for every weight.

## Return Value

A font object of the specified size and weight.

## Discussion

Instead of using this method to get a font, it’s often more appropriate to use preferredFont(forTextStyle:) because that method respects the user’s selected content size category.

## See Also

### Creating System Fonts

class func systemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in the specified size.

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

class func monospacedDigitSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the standard system font with all digits of consistent width.

