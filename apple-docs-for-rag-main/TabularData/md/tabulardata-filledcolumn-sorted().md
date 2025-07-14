

- TabularData
- FilledColumn
-  sorted() 

Instance Method

# sorted()

Returns the elements of the sequence, sorted.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted() -> [Self.Element]
```

Available when `Element` conforms to `Comparable`.

## Return Value

A sorted array of the sequence’s elements.

## Discussion

You can sort any sequence of elements that conform to the `Comparable` protocol by calling this method. Elements are sorted in ascending order.

Here’s an example of sorting a list of students’ names. Strings in Swift conform to the `Comparable` protocol, so the names are sorted in ascending order according to the less-than operator (`

```
let students: Set = ["Kofi", "Abena", "Peter", "Kweku", "Akosua"]
let sortedStudents = students.sorted()
print(sortedStudents)
// Prints "["Abena", "Akosua", "Kofi", "Kweku", "Peter"]"
```

To sort the elements of your sequence in descending order, pass the greater-than operator (`>`) to the `sorted(by:)` method.

```
let descendingStudents = students.sorted(by: >)
print(descendingStudents)
// Prints "["Peter", "Kweku", "Kofi", "Akosua", "Abena"]"
```

The sorting algorithm is guaranteed to be stable. A stable sort preserves the relative order of elements that compare as equal.

Complexity

O(*n* log *n*), where *n* is the length of the sequence.

## See Also

### Generating Arrays

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

func filter((Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func flatMap&lt;SegmentOfResult>((Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element]

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

