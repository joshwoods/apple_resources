

- UIKit
- UILetterformAwareAdjusting
-  sizingRule 

Instance Property

# sizingRule

The typographic bounds-sizing behavior that handles text with fonts that contain oversize characters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var sizingRule: UILetterformAwareSizingRule { get set }
```

**Required**

## Discussion

For more information on sizing behaviors, see UILetterformAwareAdjusting.

## See Also

### Sizing the label’s text

var adjustsFontSizeToFitWidth: Bool

A Boolean value that determines whether the label reduces the text’s font size to fit the title string into the label’s bounding rectangle.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that determines whether the label tightens text before truncating.

var baselineAdjustment: UIBaselineAdjustment

An option that controls whether the text’s baseline remains fixed when text needs to shrink to fit in the label.

var minimumScaleFactor: CGFloat

The minimum scale factor for the label’s text.

var numberOfLines: Int

The maximum number of lines for rendering text.

