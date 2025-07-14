

- JavaScriptCore
- JSStaticValue
-  init(name:getProperty:setProperty:attributes:) 

Initializer

# init(name:getProperty:setProperty:attributes:)

Creates a static value with the specified values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
init(
    name: UnsafePointer!,
    getProperty: JSObjectGetPropertyCallback!,
    setProperty: JSObjectSetPropertyCallback!,
    attributes: JSPropertyAttributes
)
```

## See Also

### Creating a Static Value

init()

Creates a static value.

