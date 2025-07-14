

- JavaScriptCore
- JSClassDefinition
-  init(version:attributes:className:parentClass:staticValues:staticFunctions:initialize:finalize:hasProperty:getProperty:setProperty:deleteProperty:getPropertyNames:callAsFunction:callAsConstructor:hasInstance:convertToType:) 

Initializer

# init(version:attributes:className:parentClass:staticValues:staticFunctions:initialize:finalize:hasProperty:getProperty:setProperty:deleteProperty:getPropertyNames:callAsFunction:callAsConstructor:hasInstance:convertToType:)

Creates a class definition with the specified values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
init(
    version: Int32,
    attributes: JSClassAttributes,
    className: UnsafePointer!,
    parentClass: JSClassRef!,
    staticValues: UnsafePointer!,
    staticFunctions: UnsafePointer!,
    initialize: JSObjectInitializeCallback!,
    finalize: JSObjectFinalizeCallback!,
    hasProperty: JSObjectHasPropertyCallback!,
    getProperty: JSObjectGetPropertyCallback!,
    setProperty: JSObjectSetPropertyCallback!,
    deleteProperty: JSObjectDeletePropertyCallback!,
    getPropertyNames: JSObjectGetPropertyNamesCallback!,
    callAsFunction: JSObjectCallAsFunctionCallback!,
    callAsConstructor: JSObjectCallAsConstructorCallback!,
    hasInstance: JSObjectHasInstanceCallback!,
    convertToType: JSObjectConvertToTypeCallback!
)
```

## See Also

### Creating a Class Definition

init()

Creates an empty class definition.

typealias JSClassAttributes

A set of JavaScript class attributes.

