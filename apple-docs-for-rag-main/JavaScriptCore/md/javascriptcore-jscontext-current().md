

- JavaScriptCore
- JSContext
-  current() 

Type Method

# current()

Returns the context currently executing JavaScript code.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class func current() -> JSContext!
```

## Return Value

The currently executing context, or `nil` if not within native code called from JavaScript.

## Discussion

Call this method within an Objective-C or Swift block or method invoked from within JavaScript to obtain the JSContext object responsible for executing that Javascript code.

If not currently in code invoked as a callback from JavaScript, this method returns `nil`.

## See Also

### Inspecting callback state in a running context

class func currentCallee() -> JSValue!

Returns the currently executing JavaScript function.

class func currentThis() -> JSValue!

Returns the value of the `this` keyword in currently executing JavaScript code.

class func currentArguments() -> [Any]!

Returns the arguments to the current native callback from JavaScript code.

