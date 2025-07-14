

- JavaScriptCore
-  JSObjectCallAsFunctionCallback 

Type Alias

# JSObjectCallAsFunctionCallback

The callback type for calling an object as a function.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSObjectCallAsFunctionCallback = (JSContextRef?, JSObjectRef?, JSObjectRef?, Int, UnsafePointer?, UnsafeMutablePointer?) -> JSValueRef?
```

## Parameters 

`ctx`  

The execution context to use.

`function`  

A JSObjectRef that is the function to call.

`thisObject`  

A JSObjectRef that is the `this` variable in the function’s scope.

`argumentCount`  

An integer count of the number of arguments in `arguments`.

`arguments`  

A `JSValue` array of the arguments to pass to the function.

`exception`  

A pointer to a JSValueRef to return an exception in, if any.

## Return Value

A JSValueRef that is the function’s return value.

## Discussion

If you name your function `CallAsFunction`, you declare it like this:

```
JSValueRef CallAsFunction(JSContextRef ctx, JSObjectRef function, JSObjectRef thisObject, size_t argumentCount, const JSValueRef arguments[], JSValueRef* exception);
```

If the JavaScript expression `myObject.myFunction()` invokes your callback, it sets `function` to `myFunction`, and `thisObject` to `myObject`.

If this callback is `NULL`, calling your object as a function throws an exception.

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

typealias JSObjectGetPropertyNamesCallback

The callback type for collecting the names of an object’s properties.

var callAsFunction: JSObjectCallAsFunctionCallback!

The callback for calling an object as a function.

