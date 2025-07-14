

- Swift
- ContiguousArray
-  sort() 

Instance Method

# sort()

Sorts the collection in place.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func sort()
```

Available when `Self` conforms to `RandomAccessCollection` and `Element` conforms to `Comparable`.

## Discussion

You can sort any mutable collection of elements that conform to the `Comparable` protocol by calling this method. Elements are sorted in ascending order.

Here’s an example of sorting a list of students’ names. Strings in Swift conform to the `Comparable` protocol, so the names are sorted in ascending order according to the less-than operator (`

```
var students = ["Kofi", "Abena", "Peter", "Kweku", "Akosua"]
students.sort()
print(students)
// Prints "["Abena", "Akosua", "Kofi", "Kweku", "Peter"]"
```

To sort the elements of your collection in descending order, pass the greater-than operator (`>`) to the `sort(by:)` method.

```
students.sort(by: >)
print(students)
// Prints "["Peter", "Kweku", "Kofi", "Akosua", "Abena"]"
```

The sorting algorithm is guaranteed to be stable. A stable sort preserves the relative order of elements that compare as equal.

Complexity

O(*n* log *n*), where *n* is the length of the collection.

