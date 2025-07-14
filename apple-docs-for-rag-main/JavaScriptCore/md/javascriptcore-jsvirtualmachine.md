

- JavaScriptCore
-  JSVirtualMachine 

Class

# JSVirtualMachine

A self-contained environment for JavaScript execution.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class JSVirtualMachine
```

## Overview

You use this class for two main purposes: to support concurrent JavaScript execution, and to manage memory for objects that bridge between JavaScript and Objective-C or Swift.

### Support Threading and Concurrent JavaScript Execution

Each JavaScript context (a JSContext object) belongs to a virtual machine. Each virtual machine can encompass multiple contexts, allowing values (JSValue objects) to pass between contexts. However, each virtual machine is distinct—you can’t pass a value that you create in one virtual machine to a context in another virtual machine.

The JavaScriptCore API is thread-safe—for example, you can create JSValue objects or evaluate scripts from any thread—however, all other threads attempting to use the same virtual machine must wait. To run JavaScript concurrently on multiple threads, use a separate JSVirtualMachine instance for each thread.

### Manage Memory for Exported Objects

When you export an Objective-C or Swift object to JavaScript, you must not to store JavaScript values in that object. This action creates a retain cycle—JSValue objects hold strong references to their enclosing JavaScript contexts, and JSContext objects hold strong references to the native objects you export to JavaScript. Instead, use the JSManagedValue class to conditionally retain a JavaScript value, and report the native ownership chain for that managed value to the JavaScriptCore virtual machine. Use the addManagedReference(_:withOwner:) and removeManagedReference(_:withOwner:) methods to describe your native object graph to JavaScriptCore. After you remove the last managed reference for an object, the JavaScript garbage collector can safely destroy that object.

## Topics

### Creating a JavaScript Virtual Machine

init!()

Initializes a JavaScript virtual machine.

### Managing Memory for Bridged Values

func addManagedReference(Any!, withOwner: Any!)

Notifies the JavaScriptCore virtual machine of an external object relationship.

func removeManagedReference(Any!, withOwner: Any!)

Notifies the JavaScriptCore virtual machine that a previously registered object relationship no longer exists.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Execution Environment

class JSContext

A JavaScript execution environment.

