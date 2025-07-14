

- UIKit
- UILabel
-  isHighlighted 

Instance Property

# isHighlighted

A Boolean value that determines whether the label draws its text with a highlight.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isHighlighted: Bool { get set }
```

## Discussion

Setting this property causes the label to redraw with the appropriate highlight state. A subclass implementing a text button might set this property to true when the user presses the button and set it to false at other times. In order for the label to draw the highlight, the highlightedTextColor property must contain a non-`nil` value.

The default value of this property is false.

## See Also

### Managing highlight values

var highlightedTextColor: UIColor?

The highlight color for the label’s text.

