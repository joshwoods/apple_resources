

- JavaScriptCore
-  JSStaticValue 

Structure

# JSStaticValue

A statically declared value property.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct JSStaticValue
```

## Topics

### Creating a Static Value

init()

Creates a static value.

init(name: UnsafePointer&lt;CChar>!, getProperty: JSObjectGetPropertyCallback!, setProperty: JSObjectSetPropertyCallback!, attributes: JSPropertyAttributes)

Creates a static value with the specified values.

### Accessing Static Value Information

var name: UnsafePointer&lt;CChar>!

A null-terminated UTF-8 string that contains the property’s name.

var getProperty: JSObjectGetPropertyCallback!

A callback to invoke when getting the property’s value.

var setProperty: JSObjectSetPropertyCallback!

A callback to invoke when setting the property’s value.

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

var staticFunctions: UnsafePointer&lt;JSStaticFunction>!

An array that contains the class’s statically declared function properties.

struct JSStaticFunction

A statically declared function property.

