

- Core Foundation
-  CFBinaryHeapContainsValue(\_:\_:) 

Function

# CFBinaryHeapContainsValue(\_:\_:)

Returns whether a given value is in a binary heap.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBinaryHeapContainsValue(
    _ heap: CFBinaryHeap!,
    _ value: UnsafeRawPointer!
) -> Bool
```

## Parameters 

`heap`  

The binary heap to search.

`value`  

The value for which to find matches in the binary heap. The compare callback provided in the CFBinaryHeapCallBacks structure when the binary heap was created is used to compare values. If `value`, or any of the values in the binary heap, are not understood by the compare callback, the behavior is undefined.

## Return Value

`true` if `value` is a member of `heap`, `false` otherwise.

## See Also

### CFBinaryHeap Miscellaneous Functions

func CFBinaryHeapAddValue(CFBinaryHeap!, UnsafeRawPointer!)

Adds a value to a binary heap.

func CFBinaryHeapApplyFunction(CFBinaryHeap!, ((UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!, UnsafeMutableRawPointer!)

Iteratively applies a function to all the values in a binary heap.

func CFBinaryHeapCreate(CFAllocator!, CFIndex, UnsafePointer&lt;CFBinaryHeapCallBacks>!, UnsafePointer&lt;CFBinaryHeapCompareContext>!) -> CFBinaryHeap!

Creates a new mutable or fixed-mutable binary heap.

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

