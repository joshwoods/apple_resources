

- Foundation
- NSPointerFunctions
- NSPointerFunctions.Options
-  opaqueMemory 

Type Property

# opaqueMemory

Take no action when pointers are deleted.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var opaqueMemory: NSPointerFunctions.Options { get }
```

## Discussion

This is usually the preferred memory option for holding arbitrary pointers.

This is essentially a no-op relinquish function; the acquire function is only used for copy-in operations. This option is unlikely a to be a good choice for objects.

## See Also

### Memory Options

static var machVirtualMemory: NSPointerFunctions.Options

Use Mach memory.

static var mallocMemory: NSPointerFunctions.Options

Use `free()` on removal, `calloc()` on copy in.

static var strongMemory: NSPointerFunctions.Options

Use strong write-barriers to backing store; use garbage-collected memory on copy-in.

static var weakMemory: NSPointerFunctions.Options

Uses weak read and write barriers appropriate for ARC or GC. Using NSPointerFunctionsWeakMemory object references will turn to `NULL` on last release.

static var machVirtualMemory: NSPointerFunctions.Options

Use Mach memory.

static var mallocMemory: NSPointerFunctions.Options

Use `free()` on removal, `calloc()` on copy in.

static var strongMemory: NSPointerFunctions.Options

Use strong write-barriers to backing store; use garbage-collected memory on copy-in.

static var weakMemory: NSPointerFunctions.Options

Uses weak read and write barriers appropriate for ARC or GC. Using NSPointerFunctionsWeakMemory object references will turn to `NULL` on last release.

let NSMapTableStrongMemory: NSPointerFunctions.Options

Equivalent to strongMemory.

let NSMapTableWeakMemory: NSPointerFunctions.Options

Equivalent to weakMemory.

