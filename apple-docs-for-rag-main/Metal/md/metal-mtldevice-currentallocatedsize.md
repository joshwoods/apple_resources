

- Metal
- MTLDevice
-  currentAllocatedSize 

Instance Property

# currentAllocatedSize

The total amount of memory, in bytes, the GPU device is using for all of its resources.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var currentAllocatedSize: Int { get }
```

**Required**

## See Also

### Checking a GPU Device’s Memory

var recommendedMaxWorkingSetSize: UInt64

An approximation of how much memory, in bytes, this GPU device can allocate without affecting its runtime performance.

**Required**

var hasUnifiedMemory: Bool

A Boolean value that indicates whether the GPU shares all of its memory with the CPU.

**Required**

var maxTransferRate: UInt64

The highest theoretical rate, in bytes per second, the system can copy between system memory and the GPU’s dedicated memory (VRAM).

**Required**

