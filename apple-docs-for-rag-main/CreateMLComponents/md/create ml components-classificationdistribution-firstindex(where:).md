

- Create ML Components
- ClassificationDistribution
-  firstIndex(where:) 

Instance Method

# firstIndex(where:)

Returns the first index in which an element of the collection satisfies the given predicate.

Create ML ComponentsSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func firstIndex(where predicate: (Self.Element) throws -> Bool) rethrows -> Self.Index?
```

## Parameters 

`predicate`  

A closure that takes an element as its argument and returns a Boolean value that indicates whether the passed element represents a match.

## Return Value

The index of the first element for which `predicate` returns `true`. If no elements in the collection satisfy the given predicate, returns `nil`.

## Discussion

You can use the predicate to find an element of a type that doesn’t conform to the `Equatable` protocol or to find an element that matches particular criteria. Here’s an example that finds a student name that begins with the letter “A”:

```
let students = ["Kofi", "Abena", "Peter", "Kweku", "Akosua"]
if let i = students.firstIndex(where: { $0.hasPrefix("A") }) {
    print("\(students[i]) starts with 'A'!")
}
// Prints "Abena starts with 'A'!"
```

Complexity

O(*n*), where *n* is the length of the collection.

