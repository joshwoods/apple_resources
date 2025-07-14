

- Core ML
- MLShapedArrayProtocol
-  init(converting:) 

Initializer

# init(converting:)

Creates a shaped array type by converting another shaped array type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(converting source: T) where T : MLShapedArrayProtocol
```

## Parameters 

`source`  

An instance with a type that conforms to MLShapedArrayProtocol.

## See Also

### Creating a Shaped Array Type from Another Type

init(MLMultiArray)

Creates a shaped array type from a multiarray.

init(converting: MLMultiArray)

Creates a shaped array type by converting a multiarray.

