

- Metal
- MTLDevice
-  maxTransferRate 

Instance Property

# maxTransferRate

The highest theoretical rate, in bytes per second, the system can copy between system memory and the GPU’s dedicated memory (VRAM).

macOS 10.15+

``` source
var maxTransferRate: UInt64 { get }
```

**Required**

## Discussion

Metal calculates this value from the raw data-clock rate, and the GPU may not be able to reach this speed in real-world conditions.

Important

The maximum transfer rate for built-in GPUs is `0`.

## See Also

### Checking a GPU Device’s Memory

var currentAllocatedSize: Int

The total amount of memory, in bytes, the GPU device is using for all of its resources.

**Required**

var recommendedMaxWorkingSetSize: UInt64

An approximation of how much memory, in bytes, this GPU device can allocate without affecting its runtime performance.

**Required**

var hasUnifiedMemory: Bool

A Boolean value that indicates whether the GPU shares all of its memory with the CPU.

**Required**

