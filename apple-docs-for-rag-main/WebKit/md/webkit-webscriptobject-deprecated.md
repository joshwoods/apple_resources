

- WebKit
-  WebScriptObject Deprecated

Class

# WebScriptObject

A `WebScriptObject` object is an Objective-C wrapper for a scripting object passed to your application from the scripting environment.

macOS 10.4–10.14Deprecated

``` source
class WebScriptObject
```

## Overview

You can not create a `WebScriptObject` object directly. You get a window `WebScriptObject` object by sending windowScriptObject to your `WebView` object.

You can use key-value coding methods—for example, `setValue:forKey:` and `valueForKey:`—to get and set properties of a `WebScriptObject` object. You can also access properties by index using the setWebScriptValueAt(_:value:) and webScriptValue(at:) methods. Use the removeWebScriptKey(_:) method to remove a scripting object property.

Not all properties and methods of a class are exported. Use the setValue(_:forUndefinedKey:) and value(forUndefinedKey:) methods to intercept access to properties that are not exported. Similarly, use the invokeUndefinedMethod(fromWebScript:withArguments:) method to intercept method invocations that are not exported.

If you want access to properties and methods defined in your own classes, use the methods in the WebScripting informal protocol to specify the properties and methods the class should export to WebKit’s JavaScript environment.

Use the callWebScriptMethod(_:withArguments:) and evaluateWebScript(_:) methods to execute scripts in the scripting environment.

## Topics

### Getting and setting properties

func jsObject() -> JSObjectRef!

Returns the JavaScript object corresponding to the receiver.

func removeWebScriptKey(String!)

Removes a property from a scripting environment.

func webScriptValue(at: UInt32) -> Any!

Returns the value of a property at the specified index.

func setWebScriptValueAt(UInt32, value: Any!)

Sets the value of a property at the specified index.

### Executing scripts

func callWebScriptMethod(String!, withArguments: [Any]!) -> Any!

Returns the result of executing a method in the scripting environment.

func evaluateWebScript(String!) -> Any!

Returns the result of evaluating a script in the scripting environment.

### Raising exceptions

class func throwException(String!) -> Bool

Raises an exception in the current script execution context.

func setException(String!)

Raises a scripting environment exception in the context of the current object.

### Getting a string representation

func stringRepresentation() -> String!

Returns a string representation of the receiver.

### Instance Methods

func jsValue() -> JSValue!

## Relationships

### Inherits From

- NSObject

### Inherited By

- DOMObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

WebKit DOM Programming Topics

WebKit Objective-C Programming Guide

### Incorporating Scripts (Legacy)

WebScripting

\`WebScripting\` is an informal protocol that defines methods that classes can implement to export their interfaces to a WebScript environment such as JavaScript.

class WebUndefined

`WebUndefined` objects are simply used to represent the JavaScript “undefined” value in methods when bridging between JavaScript and Objective-C. For example, if you invoke a JavaScript function that returns the JavaScript “undefined” value, then a `WebUndefined` object is returned to the Objective-C calling context.

Deprecated

