

- JavaScriptCore
- JSContext
-  virtualMachine 

Instance Property

# virtualMachine

The JavaScript virtual machine to which the context belongs.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var virtualMachine: JSVirtualMachine! { get }
```

## Discussion

To create a context associated with a specific virtual machine, allowing JavaScript values to be passed between contexts that share the same virtual machine, use the init(virtualMachine:) initializer.

## See Also

### Working with JavaScript global state

var globalObject: JSValue!

The JavaScript global object associated with the context.

var exception: JSValue!

A JavaScript exception to be thrown in evaluation of the script.

var exceptionHandler: ((JSContext?, JSValue?) -> Void)!

A block to be invoked should evaluating a script result in a JavaScript exception being thrown.

var name: String!

A descriptive name for the context.

