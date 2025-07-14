

- Core Media
- CMBlockBuffer
-  CMBlockBuffer.Error 

Structure

# CMBlockBuffer.Error

A structure that defines block buffer errors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Error
```

## Topics

### Errors

static let badCustomBlockSource: NSError

An error that indicates an attempt to create a block buffer without a valid source.

static let badLengthParameter: NSError

An error that indicates you called a function with an invalid length parameter.

static let badOffsetParameter: NSError

An error that indicates you called a function with offset value is out of range.

static let badPointerParameter: NSError

An error that indicates a parameter is invalid.

static let blockAllocationFailed: NSError

An error that indicates you specified an invalid allocation block.

static let emptyBlockBuffer: NSError

An error that indicates you passed an empty block buffer to a function.

static let insufficientSpace: NSError

An error that indicates there’s insufficient space to perform the operation.

static let structureAllocationFailed: NSError

An error that indicates the allocation of a structure failed.

static let unallocatedBlock: NSError

An error that indicates a function encountered an unallocated block of memory.

## Relationships

### Conforms To

- Sendable

## See Also

### Data Types

struct Flags

A structure that defines feature and control flags.

struct Slice

A structure that defines a slice of a block buffer.

