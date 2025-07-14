

- Core ML
- MLMultiArray
-  init(shape:dataType:strides:) 

Initializer

# init(shape:dataType:strides:)

Creates the object with specified strides.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    shape: [Int],
    dataType: MLMultiArrayDataType,
    strides: [Int]
)
```

## Parameters 

`shape`  

The shape

`dataType`  

The data type

`strides`  

The strides.

## Discussion

The contents of the object are left uninitialized; the client must initialize it.

