

- JavaScriptCore
-  JSClassDefinition 

Structure

# JSClassDefinition

A structure that contains properties and callbacks that define a type of object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct JSClassDefinition
```

## Overview

All fields other than the version field are optional. Any pointer may be `NULL`.

The staticValues and staticFunctions arrays are the simplest and most efficient means for vending custom properties. Statically declared properties automatically service requests like getProperty, setProperty, and getPropertyNames. Property access callbacks are necessary only to implement unusual properties, like array indexes, which have unknown names at compile time.

If you name your getter function `GetX` and your setter function `SetX`, you declare a JSStaticValue array that contains `"X"` like this:

```
```

Standard JavaScript practice calls for storing function objects in prototypes so you can share them. The default JSClassRef that JSClassCreate(_:) creates follows this idiom, instantiating objects with a shared, automatically generating prototype that contains the class’s function objects. The kJSClassAttributeNoAutomaticPrototype attribute specifies that a JSClassRef doesn’t automatically generate such a prototype. The resulting JSClassRef instantiates objects with the default object prototype, and gives each instance object its own copy of the class’s function objects.

A `NULL` callback specifies that the default object callback substitutes, except in the case of hasProperty, where it specifies that getProperty substitutes.

## Topics

### Creating a Class Definition

init()

Creates an empty class definition.

init(version: Int32, attributes: JSClassAttributes, className: UnsafePointer&lt;CChar>!, parentClass: JSClassRef!, staticValues: UnsafePointer&lt;JSStaticValue>!, staticFunctions: UnsafePointer&lt;JSStaticFunction>!, initialize: JSObjectInitializeCallback!, finalize: JSObjectFinalizeCallback!, hasProperty: JSObjectHasPropertyCallback!, getProperty: JSObjectGetPropertyCallback!, setProperty: JSObjectSetPropertyCallback!, deleteProperty: JSObjectDeletePropertyCallback!, getPropertyNames: JSObjectGetPropertyNamesCallback!, callAsFunction: JSObjectCallAsFunctionCallback!, callAsConstructor: JSObjectCallAsConstructorCallback!, hasInstance: JSObjectHasInstanceCallback!, convertToType: JSObjectConvertToTypeCallback!)

Creates a class definition with the specified values.

typealias JSClassAttributes

A set of JavaScript class attributes.

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

struct JSStaticFunction

A statically declared function property.

### Managing Callbacks

var initialize: JSObjectInitializeCallback!

The callback for creating the object.

typealias JSObjectInitializeCallback

The callback type for first creating an object.

var finalize: JSObjectFinalizeCallback!

The callback for preparing the object for garbage collection.

typealias JSObjectFinalizeCallback

The callback type for finalizing an object (preparing it for garbage collection).

var hasProperty: JSObjectHasPropertyCallback!

The callback for determining whether an object has a property.

typealias JSObjectHasPropertyCallback

The callback type for determining whether an object has a property.

var getProperty: JSObjectGetPropertyCallback!

The callback for getting a property’s value.

typealias JSObjectGetPropertyCallback

The callback type for getting a property’s value.

var setProperty: JSObjectSetPropertyCallback!

The callback for setting a property’s value.

typealias JSObjectSetPropertyCallback

The callback type for setting a property’s value.

var deleteProperty: JSObjectDeletePropertyCallback!

The callback for deleting a property.

typealias JSObjectDeletePropertyCallback

The callback type for deleting a property.

var getPropertyNames: JSObjectGetPropertyNamesCallback!

The callback for collecting the names of an object’s properties.

typealias JSObjectGetPropertyNamesCallback

The callback type for collecting the names of an object’s properties.

var callAsFunction: JSObjectCallAsFunctionCallback!

The callback for calling an object as a function.

typealias JSObjectCallAsFunctionCallback

The callback type for calling an object as a function.

var hasInstance: JSObjectHasInstanceCallback!

The callback for checking whether an object is an instance of a particular type.

typealias JSObjectHasInstanceCallback

The callback type for checking whether an object is an instance of a particular type.

var callAsConstructor: JSObjectCallAsConstructorCallback!

The callback for using an object as a constructor.

typealias JSObjectCallAsConstructorCallback

The callback type for using an object as a constructor.

var convertToType: JSObjectConvertToTypeCallback!

The callback for converting an object to a particular JavaScript type.

typealias JSObjectConvertToTypeCallback

The callback type for converting an object to a particular JavaScript type.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Working with Classes

func JSClassCreate(UnsafePointer&lt;JSClassDefinition>!) -> JSClassRef!

Creates a JavaScript class.

func JSClassRelease(JSClassRef!)

Releases a JavaScript class.

func JSClassRetain(JSClassRef!) -> JSClassRef!

Retains a JavaScript class.

let kJSClassDefinitionEmpty: JSClassDefinition

A class definition structure of the current version that contains null pointers and has no attributes.

JSClassAttribute

A JavaScript class attribute.

