

- WebKit
- WKWebView
-  evaluateJavaScript(\_:in:in:completionHandler:) 

Instance Method

# evaluateJavaScript(\_:in:in:completionHandler:)

Evaluates a JavaScript string in the context of the specified frame and content world.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOS

``` source
@MainActor @preconcurrency
func evaluateJavaScript(
    _ javaScript: String,
    in frame: WKFrameInfo? = nil,
    in contentWorld: WKContentWorld,
    completionHandler: (@MainActor (Result) -> Void)? = nil
)
```

## Parameters 

`javaScript`  

The JavaScript string to evaluate.

`frame`  

The frame in which to evaluate the JavaScript code. Specify `nil` to target the main frame. If this frame is no longer valid when script evaluation begins, this method returns a WKError.Code.javaScriptInvalidFrameTarget error.

`contentWorld`  

The namespace in which to evaluate the JavaScript code. This parameter doesn’t apply to changes you make to the underlying web content, such as the document’s DOM structure. Those changes remain visible to all scripts, regardless of which content world you specify. For more information about content worlds, see WKContentWorld.

`completionHandler`  

A handler block to execute when script evaluation finishes. The method calls your block whether script evaluation completes successfully or fails. The block has no return value and takes the following parameters:

object  
The result of the script evaluation, or `nil` if an error occurred.

error  
`nil` on success, or an error object with information about the problem.

## Discussion

The evaluation of your script may change global state in a way that remains visible to subsequent JavaScript code. The changes are restricted to scripts you execute using the same WKContentWorld object. In fact, you can use this method to set up global state in the specified content world, and use that state in subsequent JavaScript code. If you do so, consider using callAsyncJavaScript(_:arguments:in:in:completionHandler:) for more flexible interactions with the JavaScript programming model.

After evaluating the script, this method executes the completion handler block with either the result of the script evaluation or an error. The completion handler always runs on the app’s main thread.

## See Also

### Executing JavaScript

func evaluateJavaScript(String, completionHandler: ((Any?, (any Error)?) -> Void)?)

Evaluates the specified JavaScript string.

func evaluateJavaScript(String, in: WKFrameInfo?, contentWorld: WKContentWorld) async throws -> Any?

Evaluates a JavaScript string in the context of the specified frame and content world.

func callAsyncJavaScript(String, arguments: [String : Any], in: WKFrameInfo?, in: WKContentWorld, completionHandler: ((Result&lt;Any, any Error>) -> Void)?)

Executes the specified string as an asynchronous JavaScript function.

func callAsyncJavaScript(String, arguments: [String : Any], in: WKFrameInfo?, contentWorld: WKContentWorld) async throws -> Any?

Executes the specified string as an asynchronous JavaScript function.

