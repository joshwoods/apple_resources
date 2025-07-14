

- JavaScriptCore
-  JSObjectInitializeCallback 

Type Alias

# JSObjectInitializeCallback

The callback type for first creating an object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSObjectInitializeCallback = (JSContextRef?, JSObjectRef?) -> Void
```

## Parameters 

`ctx`  

The execution context to use.

`object`  

The JSObjectRef to create.

## Discussion

If you name your function `Initialize`, you declare it like this:

```
void Initialize(JSContextRef ctx, JSObjectRef object);
```

Unlike the other object callbacks, the system calls the initialize callback on the least-derived class (the parent class) first, and the most-derived class last.

## See Also

### Managing Callbacks

var initialize: JSObjectInitializeCallback!

The callback for creating the object.

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

