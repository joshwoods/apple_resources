

- UIKit
- UIFont
-  boldSystemFont(ofSize:) 

Type Method

# boldSystemFont(ofSize:)

Returns the font object for standard interface items in boldface type in the specified size.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func boldSystemFont(ofSize fontSize: CGFloat) -> UIFont
```

## Parameters 

`fontSize`  

The size (in points) for the font. This value must be greater than `0.0`.

## Return Value

A font object of the specified size.

## Discussion

Instead of using this method to get a font, it’s often more appropriate to use preferredFont(forTextStyle:) because that method respects the user’s selected content size category.

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

class func italicSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in italic type in the specified size.

class func monospacedSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the fixed-width font for standard interface text in the specified size.

class func monospacedDigitSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the standard system font with all digits of consistent width.

