

- Core Media
- CMTypedTag
- CMTypedTag.Category
-  init(rawCategory:valueForTagValue:tagValueForValue:) 

Initializer

# init(rawCategory:valueForTagValue:tagValueForValue:)

Creates a new tag category instance with defined mappings between a raw and typed tag value.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    rawCategory: CMTypedTag.RawCategory,
    valueForTagValue: @escaping (CMTag.Value) -> TypedValue?,
    tagValueForValue: @escaping (TypedValue) -> CMTag.Value
)
```

## Parameters 

`rawCategory`  

A raw 64-bit identifier for the category.

`valueForTagValue`  

A mapping from an internal tag value to a typed value.

`tagValueForValue`  

A mapping from a typed value to an internal value stored in the tag.

## Discussion

Important

To ensure that your category is valid, use an existing static category listed in Creating Typed Categories rather than creating an instance yourself.

