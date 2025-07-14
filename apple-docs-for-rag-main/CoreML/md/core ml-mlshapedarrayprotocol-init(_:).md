

- Core ML
- MLShapedArrayProtocol
-  init(\_:) 

Initializer

# init(\_:)

Creates a shaped array type from a multiarray.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(_ multiArray: MLMultiArray)
```

## Parameters 

`multiArray`  

An MLMultiArray with the same underlying type as the shaped array type.

## See Also

### Creating a Shaped Array Type from Another Type

init(converting: MLMultiArray)

Creates a shaped array type by converting a multiarray.

init&lt;T>(converting: T)

Creates a shaped array type by converting another shaped array type.

