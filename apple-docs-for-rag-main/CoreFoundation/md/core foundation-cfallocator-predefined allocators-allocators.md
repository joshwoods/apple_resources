

- Core Foundation
- CFAllocator
-  Predefined Allocators 

API Collection

# Predefined Allocators

CFAllocator provides the following predefined allocators. In general, you should use `kCFAllocatorDefault` unless one of the special circumstances exist below.

## Topics

### Constants

let kCFAllocatorDefault: CFAllocator!

This is a synonym for `NULL`.

let kCFAllocatorSystemDefault: CFAllocator!

Default system allocator.

let kCFAllocatorMalloc: CFAllocator!

This allocator uses `malloc()`, `realloc()`, and `free()`.

let kCFAllocatorMallocZone: CFAllocator!

This allocator explicitly uses the default malloc zone, returned by `malloc_default_zone()`.

let kCFAllocatorNull: CFAllocator!

This allocator does nothing—it allocates no memory.

let kCFAllocatorUseContext: CFAllocator!

Special allocator argument to CFAllocatorCreate(_:_:)—it uses the functions given in the context to allocate the allocator.

