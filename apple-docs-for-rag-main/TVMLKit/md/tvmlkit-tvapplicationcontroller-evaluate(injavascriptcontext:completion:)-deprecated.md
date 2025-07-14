

- TVMLKit
- TVApplicationController
-  evaluate(inJavaScriptContext:completion:) Deprecated

Instance Method

# evaluate(inJavaScriptContext:completion:)

Evaluates a block in the JavaScript execution queue.

tvOS 9.0–18.0Deprecated

``` source
func evaluate(
    inJavaScriptContext evaluation: @escaping (JSContext) -> Void,
    completion: ((Bool) -> Void)? = nil
)
```

``` source
func evaluate(inJavaScriptContext evaluation: @escaping (JSContext) -> Void) async -> Bool
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`evaluation`  

The block to be evaluated in the JavaScript execution queue.

`completion`  

The callback after the block has been executed. true if the block was evaluated; false otherwise.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func evaluate(inJavaScriptContext evaluation: @escaping (JSContext) -> Void) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method adds a block to the JavaScript execution queue and invokes the completion block after the evaluation block has finished execution. The `context` block parameter is valid within the scope of the evaluation block and should not be referenced by the app outside the block.

## See Also

### Controlling and Handling Events

func stop()

Ends the app life cycle.

Deprecated

