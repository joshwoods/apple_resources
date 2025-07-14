

- AppKit
- NSTextLayoutFragment
-  state 

Instance Property

# state

The layout information state.

macOS 12.0+

``` source
var state: NSTextLayoutFragment.State { get }
```

## Discussion

This property is KVO-compliant.

## See Also

### Getting element information

enum State

Values that describe the possible layout states.

var rangeInElement: NSTextRange

The range inside the text element relative to the document origin.

var textElement: NSTextElement?

The parent text element.

