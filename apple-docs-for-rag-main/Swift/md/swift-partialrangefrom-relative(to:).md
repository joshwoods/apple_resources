

- Swift
- PartialRangeFrom
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

## Discussion

You can use the `relative(to:)` method to convert a range expression, which could be missing one or both of its endpoints, into a concrete range that is bounded on both sides. The following example uses this method to convert a partial range up to `4` into a half-open range, using an array instance to add the range’s lower bound.

```
let numbers = [10, 20, 30, 40, 50, 60, 70]
let upToFour = ..

The `r1` range is bounded on the lower end by `0` because that is the starting index of the `numbers` array. When the collection passed to `relative(to:)` starts with a different index, that index is used as the lower bound instead. The next example creates a slice of `numbers` starting at index `2`, and then uses the slice with `relative(to:)` to convert `upToFour` to a concrete range.

```
let numbersSuffix = numbers[2...]
// numbersSuffix == [30, 40, 50, 60, 70]

let r2 = upToFour.relative(to: numbersSuffix)
// r2 == 2..

Use this method only if you need the concrete range it produces. To access a slice of a collection using a range expression, use the collection’s generic subscript that uses a range expression as its parameter.

```
let numbersPrefix = numbers[upToFour]
// numbersPrefix == [10, 20, 30, 40]
```

