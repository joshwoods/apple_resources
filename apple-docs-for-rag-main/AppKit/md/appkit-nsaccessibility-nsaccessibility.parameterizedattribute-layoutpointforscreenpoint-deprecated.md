

- AppKit
- NSAccessibility
- NSAccessibility.ParameterizedAttribute
-  layoutPointForScreenPoint Deprecated

Type Property

# layoutPointForScreenPoint

The point in the layout area (`NSValue`) corresponding to the specified point on the screen (`NSValue`).

macOS 10.6+

``` source
static let layoutPointForScreenPoint: NSAccessibility.ParameterizedAttribute
```

Deprecated

Use of these constants is discouraged. Use the new method-based API instead. For more information, see Accessibility Programming Guide for OS X or NSAccessibilityProtocol.

## See Also

### Attribute Names

static let attributedStringForRange: NSAccessibility.ParameterizedAttribute

Does not use attributes from Appkit/AttributedString.h (`NSAttributedString`).

static let boundsForRange: NSAccessibility.ParameterizedAttribute

The rectangle (`NSValue` containing an `NSRect` value) enclosing the specified range of characters (`NSValue` containing an `NSRange` value). If the range crosses a line boundary, the returned rectangle will fully enclose all the lines of characters.

static let cellForColumnAndRow: NSAccessibility.ParameterizedAttribute

The cell at the specified row and column.

Deprecated

static let layoutSizeForScreenSize: NSAccessibility.ParameterizedAttribute

The size of the layout area in points (`NSValue`) corresponding to the specified screen size (`NSValue`).

static let lineForIndex: NSAccessibility.ParameterizedAttribute

The line number (`NSNumber`) of the specified character (`NSNumber`).

Deprecated

static let rangeForIndex: NSAccessibility.ParameterizedAttribute

The full range of characters (`NSValue` containing an `NSRange` value), including the specified character, which compose a single glyph (`NSNumber`).

static let rangeForLine: NSAccessibility.ParameterizedAttribute

The range of characters (`NSValue` containing an `NSRange` value) corresponding to the specified line number (`NSNumber`).

static let rangeForPosition: NSAccessibility.ParameterizedAttribute

The range of characters (`NSValue` containing an `NSRange` value) composing the glyph at the specified point (`NSValue` containing an `NSPoint` value).

static let rtfForRange: NSAccessibility.ParameterizedAttribute

The RTF data (`NSData`) describing the specified range of characters (`NSValue` containing an `NSRange` value).

static let screenPointForLayoutPoint: NSAccessibility.ParameterizedAttribute

The screen point (`NSValue`) corresponding to the specified point in the layout area (`NSValue`).

static let screenSizeForLayoutSize: NSAccessibility.ParameterizedAttribute

The size of the screen in points (`NSValue`) corresponding to the specified size of the layout area (`NSValue`).

static let stringForRange: NSAccessibility.ParameterizedAttribute

The substring (`NSString`) specified by the range (`NSValue` containing an `NSRange` value).

static let styleRangeForIndex: NSAccessibility.ParameterizedAttribute

The full range of characters (`NSValue` containing an `NSRange` value), including the specified character (`NSNumber`), which have the same style.

