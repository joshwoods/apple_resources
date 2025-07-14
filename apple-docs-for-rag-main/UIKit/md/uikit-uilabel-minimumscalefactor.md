

- UIKit
- UILabel
-  minimumScaleFactor 

Instance Property

# minimumScaleFactor

The minimum scale factor for the label’s text.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var minimumScaleFactor: CGFloat { get set }
```

## Discussion

If the adjustsFontSizeToFitWidth is true, use this property to specify the smallest multiplier for the current font size that yields an acceptable font size for the label’s text. If you specify a value of `0` for this property, the label doesn’t scale the text down. The default value of this property is `0`.

To reveal the text field for editing minimum scale factor in Interface Builder, choose Minimum Font Scale from the Autoshrink pop-up menu in the label’s Attributes inspector.

## See Also

### Sizing the label’s text

var adjustsFontSizeToFitWidth: Bool

A Boolean value that determines whether the label reduces the text’s font size to fit the title string into the label’s bounding rectangle.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that determines whether the label tightens text before truncating.

var baselineAdjustment: UIBaselineAdjustment

An option that controls whether the text’s baseline remains fixed when text needs to shrink to fit in the label.

var numberOfLines: Int

The maximum number of lines for rendering text.

var sizingRule: UILetterformAwareSizingRule

The typographic bounds-sizing behavior that handles text with fonts that contain oversize characters.

**Required**

