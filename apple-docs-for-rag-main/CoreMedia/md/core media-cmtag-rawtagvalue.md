

- Core Media
- CMTag
-  rawTagValue 

Instance Property

# rawTagValue

The tag’s contained value.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final let rawTagValue: CMTag.Value
```

## See Also

### Inspecting Tags

let rawCategory: CMTag.RawCategory

The raw 64-bit representation of the tag’s category.

func value&lt;T>(onlyIfMatching: CMTypedTag&lt;T>.Category) -> T?

Retrieves a tag’s value as a specific type, if and only if it matches a category.

