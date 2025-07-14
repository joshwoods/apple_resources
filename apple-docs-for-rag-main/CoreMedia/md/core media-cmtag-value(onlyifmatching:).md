

- Core Media
- CMTag
-  value(onlyIfMatching:) 

Instance Method

# value(onlyIfMatching:)

Retrieves a tag’s value as a specific type, if and only if it matches a category.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func value(onlyIfMatching category: CMTypedTag.Category) -> T? where T : Sendable
```

## Parameters 

`category`  

The category to check if the tag contains.

## Return Value

The value contained in the tag as an instance of type `T` if the category matches. Otherwise, returns `nil`.

## See Also

### Inspecting Tags

let rawCategory: CMTag.RawCategory

The raw 64-bit representation of the tag’s category.

let rawTagValue: CMTag.Value

The tag’s contained value.

