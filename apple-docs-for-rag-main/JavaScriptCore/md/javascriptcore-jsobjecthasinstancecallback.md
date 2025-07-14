

- JavaScriptCore
-  JSObjectHasInstanceCallback 

Type Alias

# JSObjectHasInstanceCallback

The callback type for checking whether an object is an instance of a particular type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSObjectHasInstanceCallback = (JSContextRef?, JSObjectRef?, JSValueRef?, UnsafeMutablePointer?) -> Bool
```

## Parameters 

`ctx`  

The execution context to use.

`constructor`  

The JSObjectRef that is the target of the `instanceof` expression.

`possibleInstance`  

The JSValueRef to test to determine if it’s an instance of `constructor`.

`exception`  

A pointer to a JSValueRef to return an exception in, if any.

## Return Value

true if `possibleInstance` is an instance of `constructor` according to the JavaScript `instanceof` expression; otherwise, false.

## Discussion

If you name your function `HasInstance`, you declare it like this:

```
bool HasInstance(JSContextRef ctx, JSObjectRef constructor, JSValueRef possibleInstance, JSValueRef* exception);
```

If the JavaScript expression `someValue instanceof myObject` invokes your callback, it sets `constructor` to `myObject`, and `possibleInstance` to `someValue`.

If this callback is `NULL`, `instanceof` expressions that target your object return false.

Standard JavaScript practice calls for objects that implement the callAsConstructor callback to implement the hasInstance callback, as well.

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

