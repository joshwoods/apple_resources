

- UIKit
- UIFont
-  UIFont.TextStyle 

Structure

# UIFont.TextStyle

Constants that describe the preferred styles for fonts.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 3.0+

``` source
struct TextStyle
```

## Overview

Pass these constants to the preferredFont(forTextStyle:) method of UIFont or the preferredFontDescriptor(withTextStyle:) method of UIFontDescriptor to retrieve the corresponding font information.

## Topics

### Constants

static let body: UIFont.TextStyle

The font for body text.

static let callout: UIFont.TextStyle

The font for callouts.

static let caption1: UIFont.TextStyle

The font for standard captions.

static let caption2: UIFont.TextStyle

The font for alternate captions.

static let footnote: UIFont.TextStyle

The font for footnotes.

static let headline: UIFont.TextStyle

The font for headings.

static let subheadline: UIFont.TextStyle

The font for subheadings.

static let largeTitle: UIFont.TextStyle

The font style for large titles.

static let extraLargeTitle: UIFont.TextStyle

The font style for extra large titles.

static let extraLargeTitle2: UIFont.TextStyle

The font style for extra extra large titles.

static let title1: UIFont.TextStyle

The font for first-level hierarchical headings.

static let title2: UIFont.TextStyle

The font for second-level hierarchical headings.

static let title3: UIFont.TextStyle

The font for third-level hierarchical headings.

### Metrics

var metrics: UIFontMetrics

The corresponding font metrics object for the text style.

### Initializers

init(rawValue: String)

Creates a text style with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

Creating self-sizing table view cells

Create table view cells that support Dynamic Type and use system spacing constraints to adjust the spacing surrounding text labels.

class func preferredFont(forTextStyle: UIFont.TextStyle) -> UIFont

Returns an instance of the system font for the specified text style with scaling for the user’s selected content size category.

class func preferredFont(forTextStyle: UIFont.TextStyle, compatibleWith: UITraitCollection?) -> UIFont

Returns an instance of the system font for the appropriate text style and traits.

init?(name: String, size: CGFloat)

Creates and returns a font object for the specified font name and size.

init(descriptor: UIFontDescriptor, size: CGFloat)

Returns a font that matches the specified font descriptor.

func withSize(CGFloat) -> UIFont

Returns a font object that is the same as the font, but has the specified size.

