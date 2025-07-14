

- Swift
- BidirectionalCollection
-  firstMatch(of:) 

Instance Method

# firstMatch(of:)

Returns the first match of the specified regex within the collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func firstMatch(of r: some RegexComponent) -> Regex.Match?
```

Available when `SubSequence` is `Substring`.

## Return Value

The first match of `regex` in the collection, or `nil` if there isn’t a match.

