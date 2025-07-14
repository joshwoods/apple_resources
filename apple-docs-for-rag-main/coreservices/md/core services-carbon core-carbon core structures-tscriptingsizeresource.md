

- Core Services
- Carbon Core
- Carbon Core Structures
-  TScriptingSizeResource 

Structure

# TScriptingSizeResource

Defines a data type to store stack and heap information. Not typically used by developers.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct TScriptingSizeResource
```

## Topics

### Initializers

init()

init(scriptingSizeFlags: Int16, minStackSize: UInt32, preferredStackSize: UInt32, maxStackSize: UInt32, minHeapSize: UInt32, preferredHeapSize: UInt32, maxHeapSize: UInt32)

### Instance Properties

var maxHeapSize: UInt32

var maxStackSize: UInt32

var minHeapSize: UInt32

var minStackSize: UInt32

var preferredHeapSize: UInt32

var preferredStackSize: UInt32

var scriptingSizeFlags: Int16

