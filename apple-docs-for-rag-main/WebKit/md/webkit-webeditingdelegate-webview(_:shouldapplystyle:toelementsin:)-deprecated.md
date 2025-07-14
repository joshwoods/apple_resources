

- WebKit
- WebEditingDelegate
-  webView(\_:shouldApplyStyle:toElementsIn:) Deprecated

Instance Method

# webView(\_:shouldApplyStyle:toElementsIn:)

Returns whether the user should be allowed to apply a style to a range of content.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    shouldApplyStyle style: DOMCSSStyleDeclaration!,
    toElementsIn range: DOMRange!
) -> Bool
```

## Parameters 

`webView`  

The web view that the user is editing.

`style`  

The style to apply.

`range`  

The range of the content.

## Return Value

true if the user should be allowed to apply the style to the content range; otherwise, false.

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

