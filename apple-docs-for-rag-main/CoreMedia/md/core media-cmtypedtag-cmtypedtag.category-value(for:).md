

- Core Media
- CMTypedTag
- CMTypedTag.Category
-  value(for:) 

Instance Method

# value(for:)

Convert a tag value into a typed value valid for this category, if possible.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func value(for tagValue: CMTag.Value) -> TypedValue?
```

## Parameters 

`tagValue`  

The tag value to convert to a typed value.

## Return Value

A value of type `TypedValue` containing the tag value, or `nil` if the tag value couldn’t be converted to a `TypedValue`.

## See Also

### Transforming Tag Values

func tagValue(for: TypedValue) -> CMTag.Value

Convert a typed value to a raw tag value for this category.

