

- JavaScriptCore
- JSStaticValue
-  name 

Instance Property

# name

A null-terminated UTF-8 string that contains the property’s name.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var name: UnsafePointer!
```

## See Also

### Accessing Static Value Information

var getProperty: JSObjectGetPropertyCallback!

A callback to invoke when getting the property’s value.

var setProperty: JSObjectSetPropertyCallback!

A callback to invoke when setting the property’s value.

var attributes: JSPropertyAttributes

A set of property attributes to give to the property.

