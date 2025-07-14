

- Swift
- UnsafeMutablePointer
-  allocate(capacity:) 

Type Method

# allocate(capacity:)

Allocates uninitialized memory for the specified number of instances of type `Pointee`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func allocate(capacity count: Int) -> UnsafeMutablePointer
```

## Parameters 

`count`  

The amount of memory to allocate, counted in instances of `Pointee`.

## Discussion

The resulting pointer references a region of memory that is bound to `Pointee` and is `count * MemoryLayout.stride` bytes in size.

The following example allocates enough new memory to store four `Int` instances and then initializes that memory with the elements of a range.

```
let intPointer = UnsafeMutablePointer.allocate(capacity: 4)
for i in 0..

When you allocate memory, always remember to deallocate once you’re finished.

```
intPointer.deallocate()
```

