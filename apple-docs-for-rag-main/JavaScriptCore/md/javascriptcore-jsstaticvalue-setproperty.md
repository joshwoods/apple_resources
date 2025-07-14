

- JavaScriptCore
- JSStaticValue
-  setProperty 

Instance Property

# setProperty

A callback to invoke when setting the property’s value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var setProperty: JSObjectSetPropertyCallback!
```

## Discussion

This value may be `NULL` if the property has the `ReadOnly` attribute.

## See Also

### Accessing Static Value Information

var name: UnsafePointer&lt;CChar>!

A null-terminated UTF-8 string that contains the property’s name.

var getProperty: JSObjectGetPropertyCallback!

A callback to invoke when getting the property’s value.

var attributes: JSPropertyAttributes

A set of property attributes to give to the property.

