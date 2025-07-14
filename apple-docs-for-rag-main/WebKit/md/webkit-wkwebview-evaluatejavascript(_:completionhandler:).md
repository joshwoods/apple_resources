

- WebKit
- WKWebView
-  evaluateJavaScript(\_:completionHandler:) 

Instance Method

# evaluateJavaScript(\_:completionHandler:)

Evaluates the specified JavaScript string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
func evaluateJavaScript(
    _ javaScriptString: String,
    completionHandler: (@MainActor (Any?, (any Error)?) -> Void)? = nil
)
```

``` source
@MainActor
func evaluateJavaScript(_ javaScriptString: String) async throws -> Any?
```

## Parameters 

`javaScriptString`  

The JavaScript string to evaluate.

`completionHandler`  

A handler block to execute when script evaluation finishes. The method calls your block whether script evaluation completes successfully or fails. The block has no return value and takes the following parameters:

object  
The result of the script evaluation, or `nil` if an error occurred.

error  
`nil` on success, or an error object with information about the problem.

## Discussion

After evaluating the script, this method executes the completion handler block with either the result of the script evaluation or an error. The completion handler always runs on the app’s main thread.

## See Also

### Executing JavaScript

func evaluateJavaScript(String, in: WKFrameInfo?, in: WKContentWorld, completionHandler: ((Result&lt;Any, any Error>) -> Void)?)

Evaluates a JavaScript string in the context of the specified frame and content world.

func evaluateJavaScript(String, in: WKFrameInfo?, contentWorld: WKContentWorld) async throws -> Any?

Evaluates a JavaScript string in the context of the specified frame and content world.

func callAsyncJavaScript(String, arguments: [String : Any], in: WKFrameInfo?, in: WKContentWorld, completionHandler: ((Result&lt;Any, any Error>) -> Void)?)

Executes the specified string as an asynchronous JavaScript function.

func callAsyncJavaScript(String, arguments: [String : Any], in: WKFrameInfo?, contentWorld: WKContentWorld) async throws -> Any?

Executes the specified string as an asynchronous JavaScript function.

