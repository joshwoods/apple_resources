

- Core Foundation
-  kCFAllocatorMalloc 

Global Variable

# kCFAllocatorMalloc

This allocator uses `malloc()`, `realloc()`, and `free()`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFAllocatorMalloc: CFAllocator!
```

## Discussion

Typically you should not use this allocator, use `kCFAllocatorDefault` instead. This allocator is useful as the `bytesDeallocator` in CFData or `contentsDeallocator` in CFString where the memory was obtained as a result of `malloc` type functions.

## See Also

### Constants

let kCFAllocatorDefault: CFAllocator!

This is a synonym for `NULL`.

let kCFAllocatorSystemDefault: CFAllocator!

Default system allocator.

let kCFAllocatorMallocZone: CFAllocator!

This allocator explicitly uses the default malloc zone, returned by `malloc_default_zone()`.

let kCFAllocatorNull: CFAllocator!

This allocator does nothing—it allocates no memory.

let kCFAllocatorUseContext: CFAllocator!

Special allocator argument to CFAllocatorCreate(_:_:)—it uses the functions given in the context to allocate the allocator.

