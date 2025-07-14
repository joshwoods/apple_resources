

- WebKit
- WebEditingDelegate
-  webView(\_:doCommandBy:) Deprecated

Instance Method

# webView(\_:doCommandBy:)

Returns whether the receiver performs a command instead of the web view.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    doCommandBy selector: Selector!
) -> Bool
```

## Parameters 

`webView`  

The web view that the user is editing.

`selector`  

The command to perform.

## Return Value

true if the receiver will perform `command`; otherwise, false.

## Discussion

Implement this method if you want to perform `command` instead of letting the web view perform `command`.

