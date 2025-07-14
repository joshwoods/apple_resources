

- Kernel
- libkern
-  Atomic Operations 

API Collection

# Atomic Operations

Increment and decrement numbers, perform compare-and-swap operations, and manipulate other data atomically.

## Topics

### Test Operations

OSTestAndClear

Bit test and clear operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSTestAndSet

Bit test and set operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

### Increment

OSIncrementAtomic

32-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSIncrementAtomic8

8-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSIncrementAtomic16

16-bit increment operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSIncrementAtomic64

64-bit increment.

### Decrement

OSDecrementAtomic

32-bit decrement operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSDecrementAtomic8

8-bit decrement operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSDecrementAtomic16

16-bit decrement operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSDecrementAtomic64

64-bit decrement.

### Compare and Swap

OSCompareAndSwap

Compare and swap operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSCompareAndSwap64

64-bit compare and swap operation.

OSCompareAndSwapPtr

Compare and swap operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

### Additions

OSAddAtomic

32-bit add operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSAddAtomic8

8-bit add operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSAddAtomic16

16-bit add operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSAddAtomic64

64-bit atomic add operation.

### Boolean Operations

OSBitAndAtomic

32-bit logical and operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitAndAtomic8

8-bit logical and operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitAndAtomic16

16-bit logical and operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitOrAtomic

32-bit logical or operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitOrAtomic8

8-bit logical or operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitOrAtomic16

16-bit logical or operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitXorAtomic

32-bit logical xor operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitXorAtomic8

8-bit logical xor operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

OSBitXorAtomic16

16-bit logical xor operation, performed atomically with respect to all devices that participate in the coherency architecture of the platform.

## See Also

### Fundamentals

Data Types

Create strings, numbers, collections, data objects, and the other standard types employed by drivers and kernel extensions.

Byte Order Utilities

Convert values between big-endian and little-endian formats.

