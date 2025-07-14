

- WebKit
- WebView
-  stringByEvaluatingJavaScript(from:) Deprecated

Instance Method

# stringByEvaluatingJavaScript(from:)

Returns the result of running a script.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func stringByEvaluatingJavaScript(from script: String!) -> String!
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`script`  

The script to run.

## Return Value

The result of running a JavaScript specified by `script`, or an empty string if the script failed.

