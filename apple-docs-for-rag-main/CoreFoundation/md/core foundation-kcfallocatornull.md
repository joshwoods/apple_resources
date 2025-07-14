

- Core Foundation
-  kCFAllocatorNull 

Global Variable

# kCFAllocatorNull

This allocator does nothing—it allocates no memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFAllocatorNull: CFAllocator!
```

## Discussion

This allocator is useful as the `bytesDeallocator` in CFData or `contentsDeallocator` in CFString where the memory should not be freed.

## See Also

### Constants

let kCFAllocatorDefault: CFAllocator!

This is a synonym for `NULL`.

let kCFAllocatorSystemDefault: CFAllocator!

Default system allocator.

let kCFAllocatorMalloc: CFAllocator!

This allocator uses `malloc()`, `realloc()`, and `free()`.

let kCFAllocatorMallocZone: CFAllocator!

This allocator explicitly uses the default malloc zone, returned by `malloc_default_zone()`.

let kCFAllocatorUseContext: CFAllocator!

Special allocator argument to CFAllocatorCreate(_:_:)—it uses the functions given in the context to allocate the allocator.

