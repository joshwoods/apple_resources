

- WebKit
- WebView
-  mediaStyle Deprecated

Instance Property

# mediaStyle

The receiver’s CSS media property.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var mediaStyle: String! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## See Also

### Getting and Setting CSS Properties

func computedStyle(for: DOMElement!, pseudoElement: String!) -> DOMCSSStyleDeclaration!

Returns the computed style of an element and its pseudo element.

var typingStyle: DOMCSSStyleDeclaration!

The receiver’s CSS typing style.

func styleDeclaration(withText: String!) -> DOMCSSStyleDeclaration!

Returns the CSS style declaration for the specified text.

func applyStyle(DOMCSSStyleDeclaration!)

Applies the CSS typing style to the current selection.

