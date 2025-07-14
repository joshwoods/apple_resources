

- Core Foundation
-  CFAllocator 

Class

# CFAllocator

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFAllocator
```

## Overview

CFAllocator is an opaque type that allocates and deallocates memory for you. You never have to allocate, reallocate, or deallocate memory directly for Core Foundation objects—and rarely should you. You pass CFAllocator objects into functions that create objects; these functions have “Create” embedded in their names, for example, `CFStringCreateWithPascalString`. The creation functions use the allocators to allocate memory for the objects they create.

## Topics

### Creating an Allocator

func CFAllocatorCreate(CFAllocator!, UnsafeMutablePointer&lt;CFAllocatorContext>!) -> Unmanaged&lt;CFAllocator>!

Creates an allocator object.

### Managing Memory with an Allocator

func CFAllocatorAllocate(CFAllocator!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

Allocates memory using the specified allocator.

func CFAllocatorDeallocate(CFAllocator!, UnsafeMutableRawPointer!)

Deallocates a block of memory with a given allocator.

func CFAllocatorGetPreferredSizeForSize(CFAllocator!, CFIndex, CFOptionFlags) -> CFIndex

Obtains the number of bytes likely to be allocated upon a specific request.

func CFAllocatorReallocate(CFAllocator!, UnsafeMutableRawPointer!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

Reallocates memory using the specified allocator.

### Getting and Setting the Default Allocator

func CFAllocatorGetDefault() -> Unmanaged&lt;CFAllocator>!

Gets the default allocator object for the current thread.

func CFAllocatorSetDefault(CFAllocator!)

Sets the given allocator as the default for the current thread.

### Getting an Allocator’s Context

func CFAllocatorGetContext(CFAllocator!, UnsafeMutablePointer&lt;CFAllocatorContext>!)

Obtains the context of the specified allocator or of the default allocator.

### Getting the CFAllocator Type ID

func CFAllocatorGetTypeID() -> CFTypeID

Returns the type identifier for the CFAllocator opaque type.

### Callbacks

typealias CFAllocatorAllocateCallBack

A prototype for a function callback that allocates memory of a requested size.

typealias CFAllocatorCopyDescriptionCallBack

A prototype for a function callback that provides a description of the specified data.

typealias CFAllocatorDeallocateCallBack

A prototype for a function callback that deallocates a block of memory.

typealias CFAllocatorPreferredSizeCallBack

A prototype for a function callback that gives the size of memory likely to be allocated, given a certain request.

typealias CFAllocatorReallocateCallBack

A prototype for a function callback that reallocates memory of a requested size for an existing block of memory.

typealias CFAllocatorReleaseCallBack

A prototype for a function callback that releases the given data.

typealias CFAllocatorRetainCallBack

A prototype for a function callback that retains the given data.

### Data Types

struct CFAllocatorContext

A structure that defines the context or operating environment for an allocator (CFAllocator) object. Every Core Foundation allocator object must have a context defined for it.

### Constants

Predefined Allocators

CFAllocator provides the following predefined allocators. In general, you should use `kCFAllocatorDefault` unless one of the special circumstances exist below.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Memory Management Programming Guide for Core Foundation

### Opaque Types

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

class CFFileDescriptor

