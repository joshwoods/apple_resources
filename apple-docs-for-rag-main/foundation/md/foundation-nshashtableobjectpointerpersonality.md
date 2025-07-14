

- Foundation
-  NSHashTableObjectPointerPersonality 

Global Variable

# NSHashTableObjectPointerPersonality

Equal to objectPointerPersonality.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSHashTableObjectPointerPersonality: NSPointerFunctions.Options
```

## See Also

### Constants

let NSHashTableStrongMemory: NSPointerFunctions.Options

Equal to strongMemory.

let NSHashTableCopyIn: NSPointerFunctions.Options

Equal to copyIn.

let NSHashTableWeakMemory: NSPointerFunctions.Options

Equal to weakMemory. Uses weak read and write barriers appropriate for ARC or GC. Using weakMemory object references will turn to `NULL` on last release.

