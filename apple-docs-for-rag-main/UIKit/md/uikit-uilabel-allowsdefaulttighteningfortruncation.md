

- UIKit
- UILabel
-  allowsDefaultTighteningForTruncation 

Instance Property

# allowsDefaultTighteningForTruncation

A Boolean value that determines whether the label tightens text before truncating.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var allowsDefaultTighteningForTruncation: Bool { get set }
```

## Discussion

When the value of this property is true, the label tightens intercharacter spacing of its text before allowing any truncation to occur. The label determines the maximum amount of tightening automatically based on the font, current line width, line break mode, and other relevant information. This autoshrinking behavior is only intended for use with a single-line label.

The default value of this property is false.

## See Also

### Related Documentation

var enablesMarqueeWhenAncestorFocused: Bool

A Boolean value that determines whether the label scrolls its text while one of its containing views has focus.

### Sizing the label’s text

var adjustsFontSizeToFitWidth: Bool

A Boolean value that determines whether the label reduces the text’s font size to fit the title string into the label’s bounding rectangle.

var baselineAdjustment: UIBaselineAdjustment

An option that controls whether the text’s baseline remains fixed when text needs to shrink to fit in the label.

var minimumScaleFactor: CGFloat

The minimum scale factor for the label’s text.

var numberOfLines: Int

The maximum number of lines for rendering text.

var sizingRule: UILetterformAwareSizingRule

The typographic bounds-sizing behavior that handles text with fonts that contain oversize characters.

**Required**

