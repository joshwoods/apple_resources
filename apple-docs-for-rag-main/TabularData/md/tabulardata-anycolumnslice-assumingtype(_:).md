

- TabularData
- AnyColumnSlice
-  assumingType(\_:) 

Instance Method

# assumingType(\_:)

Returns a slice of the underlying typed column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func assumingType(_ type: T.Type) -> DiscontiguousColumnSlice
```

## Parameters 

`type`  

The type of the slice’s underlying parent column.

## Return Value

A typed column slice.

## Discussion

When using this method, you must provide the correct underlying type.

