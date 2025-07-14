

- JavaScriptCore
-  JSObjectGetPropertyNamesCallback 

Type Alias

# JSObjectGetPropertyNamesCallback

The callback type for collecting the names of an object’s properties.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSObjectGetPropertyNamesCallback = (JSContextRef?, JSObjectRef?, JSPropertyNameAccumulatorRef?) -> Void
```

## Parameters 

`ctx`  

The execution context to use.

`object`  

The JSObjectRef with the property names to collect.

`accumulator`  

A JavaScript property name accumulator to accumulate the names of the object’s properties in.

## Discussion

If you name your function `GetPropertyNames`, you declare it like this:

```
void GetPropertyNames(JSContextRef ctx, JSObjectRef object, JSPropertyNameAccumulatorRef propertyNames);
```

JSObjectCopyPropertyNames(_:_:) and JavaScript `for-in` loops use property name accumulators.

Use JSPropertyNameAccumulatorAddName(_:_:) to add property names to `accumulator`. A class’s getPropertyNames callback only needs to provide the names of properties that the class vends through a custom getProperty or setProperty callback. The system adds other properties independently, including statically declared properties, properties that other classes vend, and properties that belong to the object’s prototype.

## See Also

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

var callAsFunction: JSObjectCallAsFunctionCallback!

The callback for calling an object as a function.

typealias JSObjectCallAsFunctionCallback

The callback type for calling an object as a function.

