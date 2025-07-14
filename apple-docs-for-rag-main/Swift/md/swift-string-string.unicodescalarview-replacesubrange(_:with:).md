

- Swift
- String
- String.UnicodeScalarView
-  replaceSubrange(\_:with:) 

Instance Method

# replaceSubrange(\_:with:)

Replaces the elements within the specified bounds with the given Unicode scalar values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func replaceSubrange(
    _ subrange: Range,
    with newElements: C
) where C : Collection, C.Element == Unicode.Scalar
```

## Parameters 

`subrange`  

The range of elements to replace. The bounds of the range must be valid indices of the view.

`newElements`  

The new Unicode scalar values to add to the string.

## Discussion

Calling this method invalidates any existing indices for use with this string.

Complexity

O(*m*), where *m* is the combined length of the view and `newElements`. If the call to `replaceSubrange(_:with:)` simply removes elements at the end of the string, the complexity is O(*n*), where *n* is equal to `bounds.count`.

