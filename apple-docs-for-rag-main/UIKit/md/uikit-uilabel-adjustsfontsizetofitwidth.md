

- UIKit
- UILabel
-  adjustsFontSizeToFitWidth 

Instance Property

# adjustsFontSizeToFitWidth

A Boolean value that determines whether the label reduces the text’s font size to fit the title string into the label’s bounding rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var adjustsFontSizeToFitWidth: Bool { get set }
```

## Discussion

Normally, the label draws the text with the font you specify in the font property. If this property is true, and the text in the text property exceeds the label’s bounding rectangle, the label reduces the font size until the text fits or it has scaled the font down to the minimum font size. The default value for this property is false. If you change it to true, be sure that you also set an appropriate minimum font scale by modifying the minimumScaleFactor property. This autoshrinking behavior is only intended for use with a single-line label.

To enable adjustsFontSizeToFitWidth in Interface Builder, choose Minimum Font Scale from the Autoshrink pop-up menu in the label’s Attributes inspector.

## See Also

### Related Documentation

var font: UIFont!

The font of the text.

var enablesMarqueeWhenAncestorFocused: Bool

A Boolean value that determines whether the label scrolls its text while one of its containing views has focus.

### Sizing the label’s text

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that determines whether the label tightens text before truncating.

var baselineAdjustment: UIBaselineAdjustment

An option that controls whether the text’s baseline remains fixed when text needs to shrink to fit in the label.

var minimumScaleFactor: CGFloat

The minimum scale factor for the label’s text.

var numberOfLines: Int

The maximum number of lines for rendering text.

var sizingRule: UILetterformAwareSizingRule

The typographic bounds-sizing behavior that handles text with fonts that contain oversize characters.

**Required**

