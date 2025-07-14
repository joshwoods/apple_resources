

- Core Media
- CMTypedTag
- CMTypedTag.Category
-  tagValue(for:) 

Instance Method

# tagValue(for:)

Convert a typed value to a raw tag value for this category.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func tagValue(for value: TypedValue) -> CMTag.Value
```

## Parameters 

`value`  

The value to convert to a tag value.

## Return Value

The typed value as a wrapped tag value.

## See Also

### Transforming Tag Values

func value(for: CMTag.Value) -> TypedValue?

Convert a tag value into a typed value valid for this category, if possible.

