

- AppKit
- NSScrubber
-  performSequentialBatchUpdates(\_:) 

Instance Method

# performSequentialBatchUpdates(\_:)

Combines multiple scrubber content updates into a single action.

macOS 10.12.2+

``` source
@MainActor
func performSequentialBatchUpdates(_ updateBlock: () -> Void)
```

## Parameters 

`updateBlock`  

A block that represents the combination of insertion, removal, moving, and reloading instructions that should be performed simultaneously.

