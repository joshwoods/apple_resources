

- Metal
- MTLDevice
-  hasUnifiedMemory 

Instance Property

# hasUnifiedMemory

A Boolean value that indicates whether the GPU shares all of its memory with the CPU.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var hasUnifiedMemory: Bool { get }
```

**Required**

## Discussion

A GPU with unified memory (true) is typically an integrated GPU. A GPU with dedicated memory (false) may take additional time to synchronize managed resources or copy data into private GPU resources.

## See Also

### Checking a GPU Device’s Memory

var currentAllocatedSize: Int

The total amount of memory, in bytes, the GPU device is using for all of its resources.

**Required**

var recommendedMaxWorkingSetSize: UInt64

An approximation of how much memory, in bytes, this GPU device can allocate without affecting its runtime performance.

**Required**

var maxTransferRate: UInt64

The highest theoretical rate, in bytes per second, the system can copy between system memory and the GPU’s dedicated memory (VRAM).

**Required**

