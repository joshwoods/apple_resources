

- FSKit
- FSVolume
-  FSVolume.PreallocateFlags 

Structure

# FSVolume.PreallocateFlags

Behavior flags for preallocation operations.

macOS 15.4+

``` source
struct PreallocateFlags
```

## Topics

### Declaring preallocation behaviors

static var contiguous: FSVolume.PreallocateFlags

Allocates contiguous space.

static var all: FSVolume.PreallocateFlags

Allocates all requested space or no space at all.

static var persist: FSVolume.PreallocateFlags

Allocates space that isn’t freed when deleting the descriptor.

static var fromEOF: FSVolume.PreallocateFlags

Allocates space from the physical end of file.

### Working with raw values

init(rawValue: UInt)

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Preallocating space

func preallocateSpace(for: FSItem, at: off_t, length: Int, flags: FSVolume.PreallocateFlags, replyHandler: (Int, (any Error)?) -> Void)

Prealocates disk space for the given item.

**Required**

