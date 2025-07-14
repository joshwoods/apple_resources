

- JavaScriptCore
- JSContext
-  currentThis() 

Type Method

# currentThis()

Returns the value of the `this` keyword in currently executing JavaScript code.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class func currentThis() -> JSValue!
```

## Return Value

The current value of the JavaScript `this` keyword, or `nil` if not within native code called from JavaScript.

## Discussion

Call this method within an Objective-C or Swift block or method invoked from within JavaScript to obtain a JSValue object representing the current value of the `this` keyword in that JavaScript code.

If not currently in code invoked as a callback from JavaScript, this method returns `nil`.

## See Also

### Inspecting callback state in a running context

class func current() -> JSContext!

Returns the context currently executing JavaScript code.

class func currentCallee() -> JSValue!

Returns the currently executing JavaScript function.

class func currentArguments() -> [Any]!

Returns the arguments to the current native callback from JavaScript code.

