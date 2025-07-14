

- WebKit
- WebFrame
-  globalContext Deprecated

Instance Property

# globalContext

The global JavaScript execution context for bridging between the WebKit and JavaScriptCore C API.

macOS 10.3–10.14Deprecated

``` source
var globalContext: JSGlobalContextRef! { get }
```

## See Also

### Getting DOM Objects

var domDocument: DOMDocument!

The web frame’s DOM document.

Deprecated

var frameElement: DOMHTMLElement!

The web view’s DOM frame element.

Deprecated

var javaScriptContext: JSContext!

The frame’s global JavaScript execution context.

Deprecated

var windowObject: WebScriptObject!

The JavaScript window object.

Deprecated

