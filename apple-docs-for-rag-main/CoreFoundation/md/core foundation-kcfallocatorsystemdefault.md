

- Core Foundation
-  kCFAllocatorSystemDefault 

Global Variable

# kCFAllocatorSystemDefault

Default system allocator.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFAllocatorSystemDefault: CFAllocator!
```

## Discussion

You rarely need to use this.

## See Also

### Constants

let kCFAllocatorDefault: CFAllocator!

This is a synonym for `NULL`.

let kCFAllocatorMalloc: CFAllocator!

This allocator uses `malloc()`, `realloc()`, and `free()`.

let kCFAllocatorMallocZone: CFAllocator!

This allocator explicitly uses the default malloc zone, returned by `malloc_default_zone()`.

let kCFAllocatorNull: CFAllocator!

This allocator does nothing—it allocates no memory.

let kCFAllocatorUseContext: CFAllocator!

Special allocator argument to CFAllocatorCreate(_:_:)—it uses the functions given in the context to allocate the allocator.

