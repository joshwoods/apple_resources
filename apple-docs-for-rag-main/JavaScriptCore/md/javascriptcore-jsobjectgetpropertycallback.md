

- JavaScriptCore
-  JSObjectGetPropertyCallback 

Type Alias

# JSObjectGetPropertyCallback

The callback type for getting a property’s value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSObjectGetPropertyCallback = (JSContextRef?, JSObjectRef?, JSStringRef?, UnsafeMutablePointer?) -> JSValueRef?
```

## Parameters 

`ctx`  

The execution context to use.

`object`  

The JSObjectRef to search for the property.

`propertyName`  

A JSStringRef that contains the name of the property to get.

`exception`  

A pointer to a JSValueRef to return an exception in, if any.

## Return Value

The property’s value if the object has the property; otherwise, `NULL`.

## Discussion

If you name your function `GetProperty`, you declare it like this:

```
JSValueRef GetProperty(JSContextRef ctx, JSObjectRef object, JSStringRef propertyName, JSValueRef* exception);
```

If this function returns `NULL`, the get request forwards to the object’s statically declared properties, then its parent class chain (which includes the default object class), and then its prototype chain.

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

