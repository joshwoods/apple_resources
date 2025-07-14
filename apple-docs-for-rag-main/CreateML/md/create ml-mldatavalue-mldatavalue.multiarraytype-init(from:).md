

- Create ML
- MLDataValue
- MLDataValue.MultiArrayType
-  init(from:) 

Initializer

# init(from:)

Creates a data-value multidimensional array from another instance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init?(from dataValue: MLDataValue)
```

## Discussion

Use this initializer to create an MLDataValue.MultiArrayType from another multiarray instance. You can confirm the data value’s underlying type by retrieving a non-`nil` value from multiArrayValue or by inspecting the type property.

