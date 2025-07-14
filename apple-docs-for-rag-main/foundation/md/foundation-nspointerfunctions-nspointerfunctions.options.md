

- Foundation
- NSPointerFunctions
-  NSPointerFunctions.Options 

Structure

# NSPointerFunctions.Options

Defines the memory and personality options for an `NSPointerFunctions` object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Options
```

## Overview

When specifying a value, you can use only one of the options listed in Memory Options, only one of the options listed in Personality Options, and any number of other options.

## Topics

### Memory Options

These options are mutually exclusive.

static var machVirtualMemory: NSPointerFunctions.Options

Use Mach memory.

static var mallocMemory: NSPointerFunctions.Options

Use `free()` on removal, `calloc()` on copy in.

static var opaqueMemory: NSPointerFunctions.Options

Take no action when pointers are deleted.

static var strongMemory: NSPointerFunctions.Options

Use strong write-barriers to backing store; use garbage-collected memory on copy-in.

static var weakMemory: NSPointerFunctions.Options

Uses weak read and write barriers appropriate for ARC or GC. Using NSPointerFunctionsWeakMemory object references will turn to `NULL` on last release.

static var machVirtualMemory: NSPointerFunctions.Options

Use Mach memory.

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

### Personality Options

These options are mutually exclusive.

static var cStringPersonality: NSPointerFunctions.Options

Use a string hash and `strcmp`; C-string ‘`%s`’ style description.

static var integerPersonality: NSPointerFunctions.Options

Use unshifted value as hash and equality.

static var objectPersonality: NSPointerFunctions.Options

Use `hash` and `isEqual` methods for hashing and equality comparisons, use the `description` method for a description.

static var objectPointerPersonality: NSPointerFunctions.Options

Use shifted pointer for the hash value and direct comparison to determine equality; use the `description` method for a description.

static var opaquePersonality: NSPointerFunctions.Options

Use shifted pointer for the hash value and direct comparison to determine equality.

static var structPersonality: NSPointerFunctions.Options

Use a memory hash and `memcmp` (using a size function that you must set—see sizeFunction).

static var cStringPersonality: NSPointerFunctions.Options

Use a string hash and `strcmp`; C-string ‘`%s`’ style description.

static var integerPersonality: NSPointerFunctions.Options

Use unshifted value as hash and equality.

static var objectPersonality: NSPointerFunctions.Options

Use `hash` and `isEqual` methods for hashing and equality comparisons, use the `description` method for a description.

static var objectPointerPersonality: NSPointerFunctions.Options

Use shifted pointer for the hash value and direct comparison to determine equality; use the `description` method for a description.

static var opaquePersonality: NSPointerFunctions.Options

Use shifted pointer for the hash value and direct comparison to determine equality.

static var structPersonality: NSPointerFunctions.Options

Use a memory hash and `memcmp` (using a size function that you must set—see sizeFunction).

let NSMapTableObjectPointerPersonality: NSPointerFunctions.Options

Equivalent to objectPointerPersonality.

### Copy Option

static var copyIn: NSPointerFunctions.Options

Use the memory acquire function to allocate and copy items on input (see acquireFunction).

static var copyIn: NSPointerFunctions.Options

Use the memory acquire function to allocate and copy items on input (see acquireFunction).

let NSMapTableCopyIn: NSPointerFunctions.Options

Equivalent to copyIn.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

