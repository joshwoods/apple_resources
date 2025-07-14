

- Swift
- BidirectionalCollection
-  prefixMatch(of:) 

Instance Method

# prefixMatch(of:)

Returns a match if this string is matched by the given regex at its start.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func prefixMatch(of regex: R) -> Regex.Match? where R : RegexComponent
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

The regular expression to match.

## Return Value

The match, if one is found. If there is no match, or a transformation in `regex` throws an error, this method returns `nil`.

