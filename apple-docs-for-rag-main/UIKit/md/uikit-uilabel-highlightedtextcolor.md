

- UIKit
- UILabel
-  highlightedTextColor 

Instance Property

# highlightedTextColor

The highlight color for the label’s text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var highlightedTextColor: UIColor? { get set }
```

## Discussion

Subclasses that use labels to implement a type of text button can use the value in this property when drawing the pressed state for the button. The label uses this value to display text whenever the isHighlighted property is true.

The default value of this property is `nil`.

## See Also

### Managing highlight values

var isHighlighted: Bool

A Boolean value that determines whether the label draws its text with a highlight.

