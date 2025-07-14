

- AppKit
- NSTextElement
-  parent 

Instance Property

# parent

A value that represents the parent element if this text element is a child of an enclosing element.

macOS 13.0+

``` source
weak var parent: NSTextElement? { get }
```

## See Also

### Accessing text elements

var isRepresentedElement: Bool

A Boolean value that indicates whether this element is in the text layout.

var childElements: [NSTextElement]

An array of zero or more child text elements.

