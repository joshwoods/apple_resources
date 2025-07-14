

- JavaScriptCore
- JSContext
-  currentCallee() 

Type Method

# currentCallee()

Returns the currently executing JavaScript function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class func currentCallee() -> JSValue!
```

## Return Value

The currently executing JavaScript function, or `nil` if not within native code called from JavaScript.

## Discussion

Call this method within an Objective-C or Swift block or method invoked from within JavaScript to obtain a JSValue object representing the JavaScript function responsible for executing that code.

If not currently in code invoked as a callback from JavaScript, this method returns `nil`.

## See Also

### Inspecting callback state in a running context

class func current() -> JSContext!

Returns the context currently executing JavaScript code.

class func currentThis() -> JSValue!

Returns the value of the `this` keyword in currently executing JavaScript code.

class func currentArguments() -> [Any]!

Returns the arguments to the current native callback from JavaScript code.

