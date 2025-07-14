

- JavaScriptCore
- JSContext
-  init() 

Initializer

# init()

Initializes a new JavaScript context.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
init!()
```

## Return Value

A new JavaScript context.

## Discussion

This initializer creates a context along with a new, independent virtual machine (a JSVirtualMachine object). You cannot pass JavaScript values (JSValue objects) between contexts in different virtual machines. To create contexts that share a virtual machine, use the init(virtualMachine:) initializer.

## See Also

### Creating JavaScript contexts

init!(virtualMachine: JSVirtualMachine!)

Creates a new JavaScript context associated with a specific virtual machine.

