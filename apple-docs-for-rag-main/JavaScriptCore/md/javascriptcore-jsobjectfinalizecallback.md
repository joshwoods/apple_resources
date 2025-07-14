

- JavaScriptCore
-  JSObjectFinalizeCallback 

Type Alias

# JSObjectFinalizeCallback

The callback type for finalizing an object (preparing it for garbage collection).

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSObjectFinalizeCallback = (JSObjectRef?) -> Void
```

## Parameters 

`object`  

The JSObjectRef to finalize.

## Discussion

You can finalize an object on any thread.

If you name your function `Finalize`, you declare it like this:

```
void Finalize(JSObjectRef object);
```

The system calls the finalize callback on the most-derived class first, and the least-derived class (the parent class) last.

You must not call any function that may cause a garbage collection or an allocation of a garbage collected object from within a JSObjectFinalizeCallback. This includes all functions that have a JSContextRef parameter.

## See Also

### Managing Callbacks

var initialize: JSObjectInitializeCallback!

The callback for creating the object.

typealias JSObjectInitializeCallback

The callback type for first creating an object.

var finalize: JSObjectFinalizeCallback!

The callback for preparing the object for garbage collection.

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

