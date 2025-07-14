

- JavaScriptCore
- JSContext
-  name 

Instance Property

# name

A descriptive name for the context.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var name: String! { get set }
```

## Discussion

This name appears when using remote debugging to examine the context.

## See Also

### Working with JavaScript global state

var globalObject: JSValue!

The JavaScript global object associated with the context.

var exception: JSValue!

A JavaScript exception to be thrown in evaluation of the script.

var exceptionHandler: ((JSContext?, JSValue?) -> Void)!

A block to be invoked should evaluating a script result in a JavaScript exception being thrown.

var virtualMachine: JSVirtualMachine!

The JavaScript virtual machine to which the context belongs.

