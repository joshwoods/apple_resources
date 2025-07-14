

- JavaScriptCore
- JSClassDefinition
-  staticValues 

Instance Property

# staticValues

An array that contains the class’s statically declared value properties.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var staticValues: UnsafePointer!
```

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

struct JSStaticValue

A statically declared value property.

var staticFunctions: UnsafePointer&lt;JSStaticFunction>!

An array that contains the class’s statically declared function properties.

struct JSStaticFunction

A statically declared function property.

