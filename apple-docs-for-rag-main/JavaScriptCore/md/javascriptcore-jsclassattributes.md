

- JavaScriptCore
-  JSClassAttributes 

Type Alias

# JSClassAttributes

A set of JavaScript class attributes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSClassAttributes = UInt32
```

## Discussion

Combine multiple attributes by performing the logical OR operation.

## See Also

### Creating a Class Definition

init()

Creates an empty class definition.

init(version: Int32, attributes: JSClassAttributes, className: UnsafePointer&lt;CChar>!, parentClass: JSClassRef!, staticValues: UnsafePointer&lt;JSStaticValue>!, staticFunctions: UnsafePointer&lt;JSStaticFunction>!, initialize: JSObjectInitializeCallback!, finalize: JSObjectFinalizeCallback!, hasProperty: JSObjectHasPropertyCallback!, getProperty: JSObjectGetPropertyCallback!, setProperty: JSObjectSetPropertyCallback!, deleteProperty: JSObjectDeletePropertyCallback!, getPropertyNames: JSObjectGetPropertyNamesCallback!, callAsFunction: JSObjectCallAsFunctionCallback!, callAsConstructor: JSObjectCallAsConstructorCallback!, hasInstance: JSObjectHasInstanceCallback!, convertToType: JSObjectConvertToTypeCallback!)

Creates a class definition with the specified values.

