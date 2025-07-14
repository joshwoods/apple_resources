

- WebKit
- WebView
-  applyStyle(\_:) 

Instance Method

# applyStyle(\_:)

Applies the CSS typing style to the current selection.

macOS

``` source
@MainActor
func applyStyle(_ style: DOMCSSStyleDeclaration!)
```

## Parameters 

`style`  

The style to apply to the current selection.

## Discussion

This method does nothing if there is no current selection or if the current selection is collapsed.

This method hides the complexities of applying styles to elements. If necessary, this method will make multiple passes over the range of the current selection to ensure that the requested style is applied to the elements in that range, and takes into account the complexities of CSS style application rules. This method also simplifies styling attributes so that the minimum number of styling directives are used to yield a given computed style.

## See Also

### Getting and Setting CSS Properties

func computedStyle(for: DOMElement!, pseudoElement: String!) -> DOMCSSStyleDeclaration!

Returns the computed style of an element and its pseudo element.

var mediaStyle: String!

The receiver’s CSS media property.

Deprecated

var typingStyle: DOMCSSStyleDeclaration!

The receiver’s CSS typing style.

func styleDeclaration(withText: String!) -> DOMCSSStyleDeclaration!

Returns the CSS style declaration for the specified text.

