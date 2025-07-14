

- JavaScriptCore
-  JSContext 

Class

# JSContext

A JavaScript execution environment.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class JSContext
```

## Overview

You create and use JavaScript contexts to evaluate JavaScript scripts from Objective-C or Swift code; to access values that JavaScript defines or calculates; and to make native objects, methods, or functions accessible to JavaScript.

## Topics

### Creating JavaScript contexts

init!()

Initializes a new JavaScript context.

init!(virtualMachine: JSVirtualMachine!)

Creates a new JavaScript context associated with a specific virtual machine.

### Making JavaScript context inspectable

var isInspectable: Bool

A Boolean value that indicates whether you can inspect the JavaScript context with Safari Web Inspector.

### Evaluating scripts

func evaluateScript(String!) -> JSValue!

Executes the specified JavaScript code.

func evaluateScript(String!, withSourceURL: URL!) -> JSValue!

Executes the specified JavaScript code, treating the specified URL as its source location.

### Inspecting callback state in a running context

class func current() -> JSContext!

Returns the context currently executing JavaScript code.

class func currentCallee() -> JSValue!

Returns the currently executing JavaScript function.

class func currentThis() -> JSValue!

Returns the value of the `this` keyword in currently executing JavaScript code.

class func currentArguments() -> [Any]!

Returns the arguments to the current native callback from JavaScript code.

### Working with JavaScript global state

var globalObject: JSValue!

The JavaScript global object associated with the context.

var exception: JSValue!

A JavaScript exception to be thrown in evaluation of the script.

var exceptionHandler: ((JSContext?, JSValue?) -> Void)!

A block to be invoked should evaluating a script result in a JavaScript exception being thrown.

var virtualMachine: JSVirtualMachine!

The JavaScript virtual machine to which the context belongs.

var name: String!

A descriptive name for the context.

### Accessing JavaScript global state with subscripts

func objectForKeyedSubscript(Any!) -> JSValue!

Returns the value of the specified JavaScript property in the context’s global object, allowing subscript getter syntax.

func setObject(Any!, forKeyedSubscript: (any NSCopying &amp; NSObjectProtocol)!)

Sets the specified JavaScript property of the context’s global object, allowing subscript setter syntax.

### Working with the C JavaScriptCore API

var jsGlobalContextRef: JSGlobalContextRef!

Returns the C representation of the JavaScript context.

init!(JSGlobalContextRef: JSGlobalContextRef!)

Creates a JavaScript context object from the equivalent C representation.

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

class JSVirtualMachine

A self-contained environment for JavaScript execution.

