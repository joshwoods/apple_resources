

- JavaScriptCore
- JSContext
-  init(virtualMachine:) 

Initializer

# init(virtualMachine:)

Creates a new JavaScript context associated with a specific virtual machine.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
init!(virtualMachine: JSVirtualMachine!)
```

## Parameters 

`virtualMachine`  

The virtual machine with which to associate the new context.

## Return Value

A new JavaScript context.

## Discussion

By default, each context has an independent virtual machine (a JSVirtualMachine object). You cannot pass JavaScript values between contexts in different virtual machines. Use this initializer to create a context that shares its virtual machine with other JavaScript contexts to allow passing JSValue objects between those contexts.

## See Also

### Creating JavaScript contexts

init!()

Initializes a new JavaScript context.

