

- WebKit
- WebFrame
-  javaScriptContext Deprecated

Instance Property

# javaScriptContext

The frame’s global JavaScript execution context.

macOS 10.3–10.14Deprecated

``` source
var javaScriptContext: JSContext! { get }
```

## Discussion

Use this method to bridge between the WebKit and Objective-C JavaScriptCore API.

## See Also

### Getting DOM Objects

var domDocument: DOMDocument!

The web frame’s DOM document.

Deprecated

var frameElement: DOMHTMLElement!

The web view’s DOM frame element.

Deprecated

var globalContext: JSGlobalContextRef!

The global JavaScript execution context for bridging between the WebKit and JavaScriptCore C API.

Deprecated

var windowObject: WebScriptObject!

The JavaScript window object.

Deprecated

