

- Metal
- MTLDevice
-  recommendedMaxWorkingSetSize 

Instance Property

# recommendedMaxWorkingSetSize

An approximation of how much memory, in bytes, this GPU device can allocate without affecting its runtime performance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.12+tvOS 16.0+visionOS 1.0+

``` source
var recommendedMaxWorkingSetSize: UInt64 { get }
```

**Required**

## Discussion

You can help the GPU maintain its performance by keeping the total memory footprint of its resources and heaps less than this threshold value.

## See Also

### Checking a GPU Device’s Memory

var currentAllocatedSize: Int

The total amount of memory, in bytes, the GPU device is using for all of its resources.

**Required**

var hasUnifiedMemory: Bool

A Boolean value that indicates whether the GPU shares all of its memory with the CPU.

**Required**

var maxTransferRate: UInt64

The highest theoretical rate, in bytes per second, the system can copy between system memory and the GPU’s dedicated memory (VRAM).

**Required**

