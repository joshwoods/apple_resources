

- Foundation
- NSPointerFunctions
- NSPointerFunctions.Options
-  machVirtualMemory 

Type Property

# machVirtualMemory

Use Mach memory.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var machVirtualMemory: NSPointerFunctions.Options { get }
```

## See Also

### Memory Options

static var mallocMemory: NSPointerFunctions.Options

Use `free()` on removal, `calloc()` on copy in.

static var opaqueMemory: NSPointerFunctions.Options

Take no action when pointers are deleted.

static var strongMemory: NSPointerFunctions.Options

Use strong write-barriers to backing store; use garbage-collected memory on copy-in.

static var weakMemory: NSPointerFunctions.Options

Uses weak read and write barriers appropriate for ARC or GC. Using NSPointerFunctionsWeakMemory object references will turn to `NULL` on last release.

static var mallocMemory: NSPointerFunctions.Options

Use `free()` on removal, `calloc()` on copy in.

static var opaqueMemory: NSPointerFunctions.Options

Take no action when pointers are deleted.

static var strongMemory: NSPointerFunctions.Options

Use strong write-barriers to backing store; use garbage-collected memory on copy-in.

static var weakMemory: NSPointerFunctions.Options

Uses weak read and write barriers appropriate for ARC or GC. Using NSPointerFunctionsWeakMemory object references will turn to `NULL` on last release.

let NSMapTableStrongMemory: NSPointerFunctions.Options

Equivalent to strongMemory.

let NSMapTableWeakMemory: NSPointerFunctions.Options

Equivalent to weakMemory.

