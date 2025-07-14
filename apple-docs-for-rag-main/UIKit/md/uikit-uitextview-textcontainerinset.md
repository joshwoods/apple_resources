

- UIKit
- UITextView
-  textContainerInset 

Instance Property

# textContainerInset

The inset of the text container’s layout area within the text view’s content area.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var textContainerInset: UIEdgeInsets { get set }
```

## Discussion

This property provides text margins for text laid out in the text view. By default the value of this property is `(8, 0, 8, 0)`.

## See Also

### Configuring layout attributes

var usesStandardTextScaling: Bool

A Boolean value that determines the rendering scale of the text.

var sizingRule: UILetterformAwareSizingRule

The typographic bounds-sizing behavior that handles text with fonts that contain oversize characters.

**Required**

