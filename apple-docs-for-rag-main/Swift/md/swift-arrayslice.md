

- Swift
-  ArraySlice 

Structure

# ArraySlice

A slice of an `Array`, `ContiguousArray`, or `ArraySlice` instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct ArraySlice
```

## Overview

The `ArraySlice` type makes it fast and efficient for you to perform operations on sections of a larger array. Instead of copying over the elements of a slice to new storage, an `ArraySlice` instance presents a view onto the storage of a larger array. And because `ArraySlice` presents the same interface as `Array`, you can generally perform the same operations on a slice as you could on the original array.

For more information about using arrays, see `Array` and `ContiguousArray`, with which `ArraySlice` shares most properties and methods.

# Slices Are Views onto Arrays

For example, suppose you have an array holding the number of absences from each class during a session.

```
let absences = [0, 2, 0, 4, 0, 3, 1, 0]
```

You want to compare the absences in the first half of the session with those in the second half. To do so, start by creating two slices of the `absences` array.

```
let midpoint = absences.count / 2

let firstHalf = absences[..

Neither the `firstHalf` nor `secondHalf` slices allocate any new storage of their own. Instead, each presents a view onto the storage of the `absences` array.

You can call any method on the slices that you might have called on the `absences` array. To learn which half had more absences, use the `reduce(_:_:)` method to calculate each sum.

```
let firstHalfSum = firstHalf.reduce(0, +)
let secondHalfSum = secondHalf.reduce(0, +)

if firstHalfSum > secondHalfSum {
    print("More absences in the first half.")
} else {
    print("More absences in the second half.")
}
// Prints "More absences in the first half."
```

Important

Long-term storage of `ArraySlice` instances is discouraged. A slice holds a reference to the entire storage of a larger array, not just to the portion it presents, even after the original array’s lifetime ends. Long-term storage of a slice may therefore prolong the lifetime of elements that are no longer otherwise accessible, which can appear to be memory and object leakage.

# Slices Maintain Indices

Unlike `Array` and `ContiguousArray`, the starting index for an `ArraySlice` instance isn’t always zero. Slices maintain the same indices of the larger array for the same elements, so the starting index of a slice depends on how it was created, letting you perform index-based operations on either a full array or a slice.

Sharing indices between collections and their subsequences is an important part of the design of Swift’s collection algorithms. Suppose you are tasked with finding the first two days with absences in the session. To find the indices of the two days in question, follow these steps:

1.  Call `firstIndex(where:)` to find the index of the first element in the `absences` array that is greater than zero.

2.  Create a slice of the `absences` array starting after the index found in step 1.

3.  Call `firstIndex(where:)` again, this time on the slice created in step 2. Where in some languages you might pass a starting index into an `indexOf` method to find the second day, in Swift you perform the same operation on a slice of the original array.

4.  Print the results using the indices found in steps 1 and 3 on the original `absences` array.

Here’s an implementation of those steps:

```
if let i = absences.firstIndex(where: { $0 > 0 }) {                 // 1
    let absencesAfterFirst = absences[(i + 1)...]                   // 2
    if let j = absencesAfterFirst.firstIndex(where: { $0 > 0 }) {   // 3
        print("The first day with absences had \(absences[i]).")    // 4
        print("The second day with absences had \(absences[j]).")
    }
}
// Prints "The first day with absences had 2."
// Prints "The second day with absences had 4."
```

In particular, note that `j`, the index of the second day with absences, was found in a slice of the original array and then used to access a value in the original `absences` array itself.

Note

To safely reference the starting and ending indices of a slice, always use the `startIndex` and `endIndex` properties instead of specific values.

## Topics

### Initializers

init&lt;S>(S)

Creates an array containing the elements of a sequence.

### Instance Properties

var capacity: Int

The total number of elements that the array can contain without allocating new storage.

### Instance Methods

func insert(Element, at: Int)

Inserts a new element at the specified position.

func remove(at: Int) -> Element

Removes and returns the element at the specified position.

func reserveCapacity(Int)

Reserves enough space to store the specified number of elements.

func withUnsafeBufferPointer&lt;R, E>((UnsafeBufferPointer&lt;Element>) throws(E) -> R) throws(E) -> R

Calls a closure with a pointer to the array’s contiguous storage.

func withUnsafeBytes&lt;R>((UnsafeRawBufferPointer) throws -> R) rethrows -> R

Calls the given closure with a pointer to the underlying bytes of the array’s contiguous storage.

func withUnsafeMutableBufferPointer&lt;R, E>((inout UnsafeMutableBufferPointer&lt;Element>) throws(E) -> R) throws(E) -> R

Calls the given closure with a pointer to the array’s mutable contiguous storage.

func withUnsafeMutableBytes&lt;R>((UnsafeMutableRawBufferPointer) throws -> R) rethrows -> R

Calls the given closure with a pointer to the underlying bytes of the array’s mutable contiguous storage.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

Equatable Implementations

ExpressibleByArrayLiteral Implementations

Hashable Implementations

MutableCollection Implementations

RandomAccessCollection Implementations

RangeReplaceableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- AccelerateBuffer
- AccelerateMutableBuffer
- BidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Collection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousBytes
- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- CustomDebugStringConvertible

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- CustomReflectable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- CustomStringConvertible

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- DataProtocol
- Equatable

  Conforms when `Element` conforms to `Hashable`.

- ExpressibleByArrayLiteral

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Hashable

  Conforms when `Element` conforms to `Hashable`.

- MutableCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- PositionScaleRange
- RandomAccessCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- RangeReplaceableCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ScaleDomain
- ScaleRange
- Sendable

  Conforms when `Element` conforms to `Copyable`, `Escapable`, and `Sendable`.

- Sequence

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

## See Also

### Related Array Types

struct ContiguousArray

A contiguously stored array.

