

- JavaScriptCore
-  JSStaticFunction 

Structure

# JSStaticFunction

A statically declared function property.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct JSStaticFunction
```

## Topics

### Creating a Static Function

init()

Creates a static function.

init(name: UnsafePointer&lt;CChar>!, callAsFunction: JSObjectCallAsFunctionCallback!, attributes: JSPropertyAttributes)

Creates a static function with the specified values.

### Accessing Static Function Information

var name: UnsafePointer&lt;CChar>!

A null-terminated UTF-8 string that contains the property’s name.

var callAsFunction: JSObjectCallAsFunctionCallback!

A callback to invoke when calling the property as a function.

var attributes: JSPropertyAttributes

A set of property attributes to give to the property.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Managing Class Information

var parentClass: JSClassRef!

A JavaScript class to set as the class’s parent class.

var className: UnsafePointer&lt;CChar>!

A null-terminated UTF-8 string that contains the class’s name.

var version: Int32

The version of the class definition structure.

var attributes: JSClassAttributes

A set of class attributes to give to the class.

var staticValues: UnsafePointer&lt;JSStaticValue>!

An array that contains the class’s statically declared value properties.

struct JSStaticValue

A statically declared value property.

var staticFunctions: UnsafePointer&lt;JSStaticFunction>!

An array that contains the class’s statically declared function properties.

