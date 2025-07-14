

- Swift
- String
-  replaceSubrange(\_:with:) 

Instance Method

# replaceSubrange(\_:with:)

Replaces the text within the specified bounds with the given characters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func replaceSubrange(
    _ subrange: Range,
    with newElements: C
) where C : Collection, C.Element == Character
```

## Parameters 

`subrange`  

The range of text to replace. The bounds of the range must be valid indices of the string.

`newElements`  

The new characters to add to the string.

## Discussion

Calling this method invalidates any existing indices for use with this string.

Complexity

O(*m*), where *m* is the combined length of the string and `newElements`. If the call to `replaceSubrange(_:with:)` simply removes text at the end of the string, the complexity is O(*n*), where *n* is equal to `bounds.count`.

## See Also

### Replacing Substrings

func replaceSubrange&lt;C, R>(R, with: C)

Replaces the specified subrange of elements with the given collection.

