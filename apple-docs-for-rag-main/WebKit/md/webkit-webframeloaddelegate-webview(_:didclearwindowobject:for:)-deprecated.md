

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didClearWindowObject:for:) Deprecated

Instance Method

# webView(\_:didClearWindowObject:for:)

Called when the JavaScript window object in a frame is ready for loading.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    didClearWindowObject windowObject: WebScriptObject!,
    for frame: WebFrame!
)
```

## Parameters 

`webView`  

The web view sending this message.

`windowObject`  

The cleared JavaScript window object.

`frame`  

The frame containing the JavaScript window object.

## Discussion

Use this method to set custom properties on the window object before the page is actually loaded. Every time a frame loads or is reloaded all DOM properties are cleared from the window object so the new page has a fresh window object to use. If the page you are loading depends on specific window object properties to exist, they should be added at this point before any scripts are executed.

