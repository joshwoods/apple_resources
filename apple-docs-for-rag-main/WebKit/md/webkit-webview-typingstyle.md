

- WebKit
- WebView
-  typingStyle 

Instance Property

# typingStyle

The receiver’s CSS typing style.

macOS

``` source
@MainActor
var typingStyle: DOMCSSStyleDeclaration! { get set }
```

## Discussion

The typing style is reset automatically when the receiver’s selection changes.

## See Also

### Getting and Setting CSS Properties

func computedStyle(for: DOMElement!, pseudoElement: String!) -> DOMCSSStyleDeclaration!

Returns the computed style of an element and its pseudo element.

var mediaStyle: String!

The receiver’s CSS media property.

Deprecated

func styleDeclaration(withText: String!) -> DOMCSSStyleDeclaration!

Returns the CSS style declaration for the specified text.

func applyStyle(DOMCSSStyleDeclaration!)

Applies the CSS typing style to the current selection.

