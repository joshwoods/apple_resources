

- Core Foundation
-  CFBinaryHeapCreate(\_:\_:\_:\_:) 

Function

# CFBinaryHeapCreate(\_:\_:\_:\_:)

Creates a new mutable or fixed-mutable binary heap.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBinaryHeapCreate(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ callBacks: UnsafePointer!,
    _ compareContext: UnsafePointer!
) -> CFBinaryHeap!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of values that can be contained by the binary heap. The binary heap starts empty and can grow to this number of values. If this parameter is `0`, the binary heap’s maximum capacity is limited only by memory.

`callBacks`  

A pointer to a CFBinaryHeapCallBacks structure initialized with the callbacks that operate on the values placed into the binary heap. If the binary heap will be holding `CFString` objects, pass the kCFStringBinaryHeapCallBacks constant. This functions makes a copy of the contents of the callbacks structure, so that a pointer to a structure on the stack can be passed in, or can be reused for multiple binary heap creations. This callbacks parameter may not be `NULL`.

`compareContext`  

Not used. Pass `NULL`.

## Return Value

A new `CFBinaryHeap` object. Ownership follows the The Create Rule.

## See Also

### CFBinaryHeap Miscellaneous Functions

func CFBinaryHeapAddValue(CFBinaryHeap!, UnsafeRawPointer!)

Adds a value to a binary heap.

func CFBinaryHeapApplyFunction(CFBinaryHeap!, ((UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!, UnsafeMutableRawPointer!)

Iteratively applies a function to all the values in a binary heap.

func CFBinaryHeapContainsValue(CFBinaryHeap!, UnsafeRawPointer!) -> Bool

Returns whether a given value is in a binary heap.

func CFBinaryHeapCreateCopy(CFAllocator!, CFIndex, CFBinaryHeap!) -> CFBinaryHeap!

Creates a new mutable or fixed-mutable binary heap with the values from a pre-existing binary heap.

func CFBinaryHeapGetCount(CFBinaryHeap!) -> CFIndex

Returns the number of values currently in a binary heap.

func CFBinaryHeapGetCountOfValue(CFBinaryHeap!, UnsafeRawPointer!) -> CFIndex

Counts the number of times a given value occurs in a binary heap.

func CFBinaryHeapGetMinimum(CFBinaryHeap!) -> UnsafeRawPointer!

Returns the minimum value in a binary heap.

func CFBinaryHeapGetMinimumIfPresent(CFBinaryHeap!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Returns the minimum value in a binary heap, if present.

func CFBinaryHeapGetTypeID() -> CFTypeID

Returns the type identifier of the `CFBinaryHeap` opaque type.

func CFBinaryHeapGetValues(CFBinaryHeap!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Copies all the values from a binary heap into a sorted C array.

func CFBinaryHeapRemoveAllValues(CFBinaryHeap!)

Removes all values from a binary heap, making it empty.

func CFBinaryHeapRemoveMinimumValue(CFBinaryHeap!)

Removes the minimum value from a binary heap.

