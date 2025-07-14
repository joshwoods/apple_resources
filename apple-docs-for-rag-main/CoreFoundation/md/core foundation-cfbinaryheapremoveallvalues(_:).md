

- Core Foundation
-  CFBinaryHeapRemoveAllValues(\_:) 

Function

# CFBinaryHeapRemoveAllValues(\_:)

Removes all values from a binary heap, making it empty.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBinaryHeapRemoveAllValues(_ heap: CFBinaryHeap!)
```

## Parameters 

`heap`  

The binary heap to use.

## See Also

### CFBinaryHeap Miscellaneous Functions

func CFBinaryHeapAddValue(CFBinaryHeap!, UnsafeRawPointer!)

Adds a value to a binary heap.

func CFBinaryHeapApplyFunction(CFBinaryHeap!, ((UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!, UnsafeMutableRawPointer!)

Iteratively applies a function to all the values in a binary heap.

func CFBinaryHeapContainsValue(CFBinaryHeap!, UnsafeRawPointer!) -> Bool

Returns whether a given value is in a binary heap.

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

func CFBinaryHeapRemoveMinimumValue(CFBinaryHeap!)

Removes the minimum value from a binary heap.

