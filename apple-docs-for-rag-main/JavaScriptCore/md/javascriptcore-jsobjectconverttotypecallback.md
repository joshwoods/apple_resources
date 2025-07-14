

- JavaScriptCore
-  JSObjectConvertToTypeCallback 

Type Alias

# JSObjectConvertToTypeCallback

The callback type for converting an object to a particular JavaScript type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSObjectConvertToTypeCallback = (JSContextRef?, JSObjectRef?, JSType, UnsafeMutablePointer?) -> JSValueRef?
```

## Parameters 

`ctx`  

The execution context to use.

`object`  

The JSObjectRef to convert.

`type`  

A JSType that specifies the JavaScript type to convert to.

`exception`  

A pointer to a JSValueRef to return an exception in, if any.

## Return Value

The object’s converted value, or `NULL` if the object doesn’t convert.

## Discussion

If you name your function `ConvertToType`, you declare it like this:

```
JSValueRef ConvertToType(JSContextRef ctx, JSObjectRef object, JSType type, JSValueRef* exception);
```

If this function returns false, the conversion request forwards to the object’s parent class chain (which includes the default object class).

The system only invokes this function when converting an object to kJSTypeNumber or kJSTypeString. An object that converts to kJSTypeBoolean is `true`. An object that converts to kJSTypeObject is itself.

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

