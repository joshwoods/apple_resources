

- Foundation
- Object Runtime
- Objective-C Garbage Collection
-  Memory Allocation Options 

API Collection

# Memory Allocation Options

Constants used to control behavior when allocating or reallocating collectible memory.

## Overview

These constants are used as components in a bitfield to specify the behavior of NSAllocateCollectable and NSReallocateCollectable.

## Topics

### Constants

var NSScannedOption: Int

Specifies allocation of scanned memory.

var NSCollectorDisabledOption: Int

Specifies that the block is retained, and therefore ineligible for collection. Specifying this option is equivalent to invoking disableCollectorForPointer: with the returned block as the argument.

## See Also

### Legacy

