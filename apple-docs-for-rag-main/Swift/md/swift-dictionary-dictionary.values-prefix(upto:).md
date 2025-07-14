

- Swift
- Dictionary
- Dictionary.Values
-  prefix(upTo:) 

Instance Method

# prefix(upTo:)

Returns a subsequence from the start of the collection up to, but not including, the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func prefix(upTo end: Self.Index) -> Self.SubSequence
```

## Parameters 

`end`  

The “past the end” index of the resulting subsequence. `end` must be a valid index of the collection.

## Return Value

A subsequence up to, but not including, the `end` position.

## Discussion

The resulting subsequence *does not include* the element at the position `end`. The following example searches for the index of the number `40` in an array of integers, and then prints the prefix of the array up to, but not including, that index:

```
let numbers = [10, 20, 30, 40, 50, 60]
if let i = numbers.firstIndex(of: 40) {
    print(numbers.prefix(upTo: i))
}
// Prints "[10, 20, 30]"
```

Passing the collection’s starting index as the `end` parameter results in an empty subsequence.

```
print(numbers.prefix(upTo: numbers.startIndex))
// Prints "[]"
```

Using the `prefix(upTo:)` method is equivalent to using a partial half-open range as the collection’s subscript. The subscript notation is preferred over `prefix(upTo:)`.

```
if let i = numbers.firstIndex(of: 40) {
    print(numbers[..

Complexity

O(1)

