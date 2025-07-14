

- Swift
- Range
-  relative(to:) 

Instance Method

# relative(to:)

Returns the range of indices described by this range expression within the given collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func relative(to collection: C) -> Range where Bound == C.Index, C : Collection
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`collection`  

The collection to evaluate this range expression in relation to.

## Return Value

A range suitable for slicing `collection`. The returned range is *not* guaranteed to be inside the bounds of `collection`. Callers should apply the same preconditions to the return value as they would to a range provided directly by the user.

## See Also

### Converting Ranges

init?(NSRange, in: String)

init?&lt;S>(NSRange, in: S)

