

- WebKit
- WebView
-  computedStyle(for:pseudoElement:) 

Instance Method

# computedStyle(for:pseudoElement:)

Returns the computed style of an element and its pseudo element.

macOS

``` source
@MainActor
func computedStyle(
    for element: DOMElement!,
    pseudoElement: String!
) -> DOMCSSStyleDeclaration!
```

## Parameters 

`element`  

The element whose computed style is returned.

`pseudoElement`  

The pseudo element for `element`.

## Return Value

An immutable object describing the computed style of `element` and `pseudoElement` according to the Cascading Style Sheets Specification at `http://www.w3.org/TR/CSS21`. Returns `nil` if the receiver doesn’t display `element`.

## See Also

### Getting and Setting CSS Properties

var mediaStyle: String!

The receiver’s CSS media property.

Deprecated

var typingStyle: DOMCSSStyleDeclaration!

The receiver’s CSS typing style.

func styleDeclaration(withText: String!) -> DOMCSSStyleDeclaration!

Returns the CSS style declaration for the specified text.

func applyStyle(DOMCSSStyleDeclaration!)

Applies the CSS typing style to the current selection.

