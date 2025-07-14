

- JavaScriptCore
- C JavaScriptCore API
- JSObjectRef
-  JSPropertyAttribute 

API Collection

# JSPropertyAttribute

A JavaScript property attribute.

## Topics

### Constants

var kJSPropertyAttributeNone: Int

An attribute that specifies that a property has no special attributes.

var kJSPropertyAttributeReadOnly: Int

An attribute that specifies that a property is read-only.

var kJSPropertyAttributeDontEnum: Int

An attribute that specifies that property enumerators and JavaScript for-in loops don’t enumerate a property.

var kJSPropertyAttributeDontDelete: Int

An attribute that specifies that the delete operation fails on a property.

## See Also

### Working with Properties

func JSPropertyNameAccumulatorAddName(JSPropertyNameAccumulatorRef!, JSStringRef!)

Adds a property name to a JavaScript property name accumulator.

func JSPropertyNameArrayGetCount(JSPropertyNameArrayRef!) -> Int

Gets a count of the number of items in a JavaScript property name array.

func JSPropertyNameArrayGetNameAtIndex(JSPropertyNameArrayRef!, Int) -> JSStringRef!

Gets a property name at a specified index in a JavaScript property name array.

func JSPropertyNameArrayRelease(JSPropertyNameArrayRef!)

Releases a JavaScript property name array.

func JSPropertyNameArrayRetain(JSPropertyNameArrayRef!) -> JSPropertyNameArrayRef!

Retains a JavaScript property name array.

typealias JSPropertyAttributes

A set of JavaScript property attributes.

typealias JSPropertyNameArrayRef

An array of JavaScript property names.

typealias JSPropertyNameAccumulatorRef

An ordered set of the names of a JavaScript object’s properties.

