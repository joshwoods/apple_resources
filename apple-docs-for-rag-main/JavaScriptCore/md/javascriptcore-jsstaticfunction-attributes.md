

- JavaScriptCore
- JSStaticFunction
-  attributes 

Instance Property

# attributes

A set of property attributes to give to the property.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var attributes: JSPropertyAttributes
```

## See Also

### Accessing Static Function Information

var name: UnsafePointer&lt;CChar>!

A null-terminated UTF-8 string that contains the property’s name.

var callAsFunction: JSObjectCallAsFunctionCallback!

A callback to invoke when calling the property as a function.

