

- WebKit
- WebFrame
-  domDocument Deprecated

Instance Property

# domDocument

The web frame’s DOM document.

macOS 10.3–10.14Deprecated

``` source
var domDocument: DOMDocument! { get }
```

## Discussion

`nil` if the receiver doesn’t have a DOM document; for example, if it’s a standalone image.

## See Also

### Getting DOM Objects

var frameElement: DOMHTMLElement!

The web view’s DOM frame element.

Deprecated

var globalContext: JSGlobalContextRef!

The global JavaScript execution context for bridging between the WebKit and JavaScriptCore C API.

Deprecated

var javaScriptContext: JSContext!

The frame’s global JavaScript execution context.

Deprecated

var windowObject: WebScriptObject!

The JavaScript window object.

Deprecated

