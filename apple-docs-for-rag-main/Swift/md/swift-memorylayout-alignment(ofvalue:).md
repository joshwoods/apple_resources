

- Swift
- MemoryLayout
-  alignment(ofValue:) 

Type Method

# alignment(ofValue:)

Returns the default memory alignment of `T`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func alignment(ofValue value: borrowing T) -> Int
```

## Parameters 

`value`  

A value representative of the type to describe.

## Return Value

The default memory alignment, in bytes, of the given value’s type. This value is always positive.

## Discussion

Use a type’s alignment when allocating memory using an unsafe pointer.

When you have a type instead of an instance, use the `MemoryLayout.stride` static property instead.

```
let x: Int = 100

// Finding the alignment of a value's type
let s = MemoryLayout.alignment(ofValue: x)
// s == 8

// Finding the alignment of a type directly
let t = MemoryLayout.alignment
// t == 8
```

## See Also

### Accessing the Layout of a Value

static func stride(ofValue: borrowing T) -> Int

Returns the number of bytes from the start of one instance of `T` to the start of the next when stored in contiguous memory or in an `Array`.

static func size(ofValue: borrowing T) -> Int

Returns the contiguous memory footprint of the given instance.

