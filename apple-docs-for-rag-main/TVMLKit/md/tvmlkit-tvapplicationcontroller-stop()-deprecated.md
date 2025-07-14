

- TVMLKit
- TVApplicationController
-  stop() Deprecated

Instance Method

# stop()

Ends the app life cycle.

tvOS 9.0–18.0Deprecated

``` source
func stop()
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

After the JavaScript context has ended and all resources have been released, appController(_:didStop:) is called. The app controller cannot be reused after the `stop` method has been called.

## See Also

### Controlling and Handling Events

func evaluate(inJavaScriptContext: (JSContext) -> Void, completion: ((Bool) -> Void)?)

Evaluates a block in the JavaScript execution queue.

Deprecated

