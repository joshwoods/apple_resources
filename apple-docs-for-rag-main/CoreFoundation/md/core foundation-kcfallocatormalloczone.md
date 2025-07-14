

- Core Foundation
-  kCFAllocatorMallocZone 

Global Variable

# kCFAllocatorMallocZone

This allocator explicitly uses the default malloc zone, returned by `malloc_default_zone()`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFAllocatorMallocZone: CFAllocator!
```

## Discussion

You should only use this when an object is safe to be allocated in non-scanned memory.

## See Also

### Constants

let kCFAllocatorDefault: CFAllocator!

This is a synonym for `NULL`.

let kCFAllocatorSystemDefault: CFAllocator!

Default system allocator.

let kCFAllocatorMalloc: CFAllocator!

This allocator uses `malloc()`, `realloc()`, and `free()`.

let kCFAllocatorNull: CFAllocator!

This allocator does nothing—it allocates no memory.

let kCFAllocatorUseContext: CFAllocator!

Special allocator argument to CFAllocatorCreate(_:_:)—it uses the functions given in the context to allocate the allocator.

