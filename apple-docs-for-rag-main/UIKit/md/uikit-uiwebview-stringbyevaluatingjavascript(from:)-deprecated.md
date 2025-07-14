

- UIKit
- UIWebView
-  stringByEvaluatingJavaScript(from:) Deprecated

Instance Method

# stringByEvaluatingJavaScript(from:)

Returns the result of running a JavaScript script.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
func stringByEvaluatingJavaScript(from script: String) -> String?
```

## Parameters 

`script`  

The JavaScript script to run.

## Return Value

The result of running the JavaScript script passed in the `script` parameter, or `nil` if the script fails.

## Discussion

New apps should instead use the evaluateJavaScript(_:completionHandler:) method from the WKWebView class. Legacy apps should adopt that method if possible.

Important

The stringByEvaluatingJavaScript(from:) method waits synchronously for JavaScript evaluation to complete. If you load web content whose JavaScript code you have not vetted, invoking this method could hang your app. Best practice is to adopt the WKWebView class and use its evaluateJavaScript(_:completionHandler:) method instead.

