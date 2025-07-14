

- Swift
- Sequence
-  filter(matchingCategory:) 

Instance Method

# filter(matchingCategory:)

Filters a sequence of tags based on matching the specified category. Returns the tags that match the specified category.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func filter(matchingCategory category: CMTypedTag.Category) -> [CMTypedTag] where T : Sendable
```

Available when `Element` inherits `CMTag`.

## Discussion

- category: The category to match.

