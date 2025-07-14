

- JavaScriptCore
- JSContext
-  currentArguments() 

Type Method

# currentArguments()

Returns the arguments to the current native callback from JavaScript code.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class func currentArguments() -> [Any]!
```

## Return Value

The current callback arguments, or `nil` if not within native code called from JavaScript.

## Discussion

Call this method within an Objective-C or Swift block or method invoked from within JavaScript to obtain an array of JSValue objects representing the arguments to the JavaScript function responsible for that callback.

If not currently in code invoked as a callback from JavaScript, this method returns `nil`.

## See Also

### Inspecting callback state in a running context

class func current() -> JSContext!

Returns the context currently executing JavaScript code.

class func currentCallee() -> JSValue!

Returns the currently executing JavaScript function.

class func currentThis() -> JSValue!

Returns the value of the `this` keyword in currently executing JavaScript code.

