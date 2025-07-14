

- UIKit
- UITextView
-  layoutManager 

Instance Property

# layoutManager

The layout manager that lays out text for the text view’s text container.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var layoutManager: NSLayoutManager { get }
```

## Discussion

This property is a convenience accessor that provides access through the text container.

## See Also

### Accessing TextKit Objects

var textLayoutManager: NSTextLayoutManager?

The text layout manager that lays out text for the text view’s text container.

var textContainer: NSTextContainer

The text container object that defines the area where text displays in the text view.

var textStorage: NSTextStorage

The text storage object holding the text that displays in the text view.

