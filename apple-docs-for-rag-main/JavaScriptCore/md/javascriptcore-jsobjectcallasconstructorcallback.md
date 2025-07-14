

- JavaScriptCore
-  JSObjectCallAsConstructorCallback 

Type Alias

# JSObjectCallAsConstructorCallback

The callback type for using an object as a constructor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSObjectCallAsConstructorCallback = (JSContextRef?, JSObjectRef?, Int, UnsafePointer?, UnsafeMutablePointer?) -> JSObjectRef?
```

## Parameters 

`ctx`  

The execution context to use.

`constructor`  

A JSObjectRef that is the constructor to call.

`argumentCount`  

An integer count of the number of arguments in `arguments`.

`arguments`  

A JSValueRef array of the arguments to pass to the function.

`exception`  

A pointer to a JSValueRef to return an exception in, if any.

## Return Value

A JSObjectRef that is the constructor’s return value.

## Discussion

If you name your function `CallAsConstructor`, you declare it like this:

```
JSObjectRef CallAsConstructor(JSContextRef ctx, JSObjectRef constructor, size_t argumentCount, const JSValueRef arguments[], JSValueRef* exception);
```

If the JavaScript expression `new myConstructor()` invokes your callback, it sets `constructor` to `myConstructor`.

If this callback is `NULL`, using your object as a constructor in a `new` expression throws an exception.

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

