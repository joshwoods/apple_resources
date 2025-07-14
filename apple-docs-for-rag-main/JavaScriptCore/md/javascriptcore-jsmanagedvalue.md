

- JavaScriptCore
-  JSManagedValue 

Class

# JSManagedValue

A JavaScript value with conditional retain behavior to provide automatic memory management.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class JSManagedValue
```

## Overview

The primary use case for a managed value is to store a JavaScript value in an Objective-C or Swift object that exports to JavaScript.

Important

Don’t store a nonmanaged JSValue object in a native object that exports to JavaScript. Because a JSValue object references its enclosing JSContext object, this action creates a retain cycle, preventing deallocation of the context.

A managed value’s *conditional retain* behavior ensures retention of its underlying JavaScript value as long as either of the following conditions is true:

- The JavaScript value is reachable through the JavaScript object graph (that is, not subject to JavaScript garbage collection).

- The JSManagedValue object is reachable through the Objective-C or Swift object graph, as you report to the JavaScriptCore virtual machine using the addManagedReference(_:withOwner:) method.

However, if neither of these conditions is true, the managed value sets its value property to `nil`, releasing the underlying JSValue object.

Note

On its own, a JSManagedValue object behaves similarly to an ARC weak reference to its underlying JSValue object—that is, if you don’t use the addManagedReference(_:withOwner:) method to add conditional retain behavior, the managed value’s value property automatically becomes `nil` when the JavaScript garbage collector destroys the underlying JavaScript value.

## Topics

### Creating a Managed Value

init!(value: JSValue!)

Initializes a managed value with the specified JavaScript value.

init!(value: JSValue!, andOwner: Any!)

Creates a managed value and associates it with an owner.

### Accessing the Managed Value

var value: JSValue!

The managed value’s underlying JavaScript value.

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

### JavaScript Code

class JSValue

A JavaScript value.

