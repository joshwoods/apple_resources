

- Security
-  SecTransformAttributeActionBlock Deprecated

Type Alias

# SecTransformAttributeActionBlock

A block used to override the default attribute handling for when an attribute is set.

macOS 10.7–13.0Deprecated

``` source
typealias SecTransformAttributeActionBlock = (SecTransformAttribute, CFTypeRef) -> Unmanaged?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`attribute`  

The attribute whose default is being overridden or NULL if this is a generic notification override

`value`  

Proposed new value for the attribute.

## Return Value

The new value of the attribute if successful or a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 object on failure. If a transform needs to have a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 as the value of an attribute, then place the object in a container, such as a CFArray or CFDictionary object.

