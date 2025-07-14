

- Foundation
-  NSHashTableOptions 

Type Alias

# NSHashTableOptions

Components in a bit-field to specify the behavior of elements in an NSHashTable object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias NSHashTableOptions = Int
```

## Topics

### Constants

let NSHashTableStrongMemory: NSPointerFunctions.Options

Equal to strongMemory.

let NSHashTableCopyIn: NSPointerFunctions.Options

Equal to copyIn.

let NSHashTableObjectPointerPersonality: NSPointerFunctions.Options

Equal to objectPointerPersonality.

let NSHashTableWeakMemory: NSPointerFunctions.Options

Equal to weakMemory. Uses weak read and write barriers appropriate for ARC or GC. Using weakMemory object references will turn to `NULL` on last release.

