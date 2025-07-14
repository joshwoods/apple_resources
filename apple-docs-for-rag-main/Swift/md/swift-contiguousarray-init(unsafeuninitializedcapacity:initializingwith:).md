

- Swift
- ContiguousArray
-  init(unsafeUninitializedCapacity:initializingWith:) 

Initializer

# init(unsafeUninitializedCapacity:initializingWith:)

Creates an array with the specified capacity, then calls the given closure with a buffer covering the array’s uninitialized memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    unsafeUninitializedCapacity: Int,
    initializingWith initializer: (inout UnsafeMutableBufferPointer, inout Int) throws -> Void
) rethrows
```

## Parameters 

`unsafeUninitializedCapacity`  

The number of elements to allocate space for in the new array.

`initializer`  

A closure that initializes elements and sets the count of the new array.

- Parameters:

  - buffer: A buffer covering uninitialized memory with room for the specified number of elements.

  - initializedCount: The count of initialized elements in the array, which begins as zero. Set `initializedCount` to the number of elements you initialize.

## Discussion

Inside the closure, set the `initializedCount` parameter to the number of elements that are initialized by the closure. The memory in the range `buffer[0..

