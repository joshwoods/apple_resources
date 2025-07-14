

- UIKit
- UIFontDescriptor
- UIFontDescriptor.AttributeName
-  cascadeList 

Type Property

# cascadeList

The cascading list attribute.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
static let cascadeList: UIFontDescriptor.AttributeName
```

## Discussion

The value is an NSArray instance, where each member of the array is a subdescriptor. The default value is the system default cascading list for the user’s locale.

## See Also

### Constants

static let characterSet: UIFontDescriptor.AttributeName

The character set attribute.

static let face: UIFontDescriptor.AttributeName

The font face attribute.

static let family: UIFontDescriptor.AttributeName

The font family attribute.

static let featureSettings: UIFontDescriptor.AttributeName

The font feature settings attribute.

static let fixedAdvance: UIFontDescriptor.AttributeName

The glyph advancement attribute.

static let matrix: UIFontDescriptor.AttributeName

The font’s transformation matrix attribute.

static let name: UIFontDescriptor.AttributeName

The font name attribute.

static let size: UIFontDescriptor.AttributeName

The font size attribute.

static let textStyle: UIFontDescriptor.AttributeName

The text style attribute.

static let traits: UIFontDescriptor.AttributeName

The font traits dictionary attribute.

static let visibleName: UIFontDescriptor.AttributeName

The font’s visible name attribute.

