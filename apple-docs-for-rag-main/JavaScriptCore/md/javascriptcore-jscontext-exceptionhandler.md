

- JavaScriptCore
- JSContext
-  exceptionHandler 

Instance Property

# exceptionHandler

A block to be invoked should evaluating a script result in a JavaScript exception being thrown.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var exceptionHandler: ((JSContext?, JSValue?) -> Void)! { get set }
```

## Discussion

The block takes the following parameters:

context  
The context in which the exception originates.

exception  
The JavaScript exception thrown.

The default value exception handler block stores its `exception` parameter value into the context’s exception property. As a consequence, the default behavior is that unhandled exceptions occurring within a callback from JavaScript to native code are thrown again upon return. Setting this value to `nil` results in all uncaught exceptions being silently consumed.

## See Also

### Working with JavaScript global state

var globalObject: JSValue!

The JavaScript global object associated with the context.

var exception: JSValue!

A JavaScript exception to be thrown in evaluation of the script.

var virtualMachine: JSVirtualMachine!

The JavaScript virtual machine to which the context belongs.

var name: String!

A descriptive name for the context.

