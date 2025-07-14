

- WebKit
- WebView
-  styleDeclaration(withText:) 

Instance Method

# styleDeclaration(withText:)

Returns the CSS style declaration for the specified text.

macOS

``` source
@MainActor
func styleDeclaration(withText text: String!) -> DOMCSSStyleDeclaration!
```

## Parameters 

`text`  

The text whose style declaration is returned.

## Return Value

The style declaration for `text`.

## See Also

### Getting and Setting CSS Properties

func computedStyle(for: DOMElement!, pseudoElement: String!) -> DOMCSSStyleDeclaration!

Returns the computed style of an element and its pseudo element.

var mediaStyle: String!

The receiver’s CSS media property.

Deprecated

var typingStyle: DOMCSSStyleDeclaration!

The receiver’s CSS typing style.

func applyStyle(DOMCSSStyleDeclaration!)

Applies the CSS typing style to the current selection.

