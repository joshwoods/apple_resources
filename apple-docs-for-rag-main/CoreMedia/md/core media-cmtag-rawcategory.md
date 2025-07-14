

- Core Media
- CMTag
-  rawCategory 

Instance Property

# rawCategory

The raw 64-bit representation of the tag’s category.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final let rawCategory: CMTag.RawCategory
```

## See Also

### Inspecting Tags

let rawTagValue: CMTag.Value

The tag’s contained value.

func value&lt;T>(onlyIfMatching: CMTypedTag&lt;T>.Category) -> T?

Retrieves a tag’s value as a specific type, if and only if it matches a category.

