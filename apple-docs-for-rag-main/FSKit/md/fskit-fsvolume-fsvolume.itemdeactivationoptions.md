

- FSKit
- FSVolume
-  FSVolume.ItemDeactivationOptions 

Structure

# FSVolume.ItemDeactivationOptions

Options to specify the item deactivation policy.

macOS 15.4+

``` source
struct ItemDeactivationOptions
```

## Overview

Callers may want to set a deactivation policy because deactivateItem(_:replyHandler:) processing blocks the kernel. Setting a deactivation policy allows the file system to take action at a definitive point in the item’s life cycle. These options allow the file system to instruct the FSKit kernel of which circumstances require the expense of a round-trip call to the module.

Note

To avoid performing deactivation calls, Objective-C developers use the value `FSItemDeactivationNever`. In Swift, use an empty option set (`[]`).

## Topics

### Declaring deactivation options

static var forRemovedItems: FSVolume.ItemDeactivationOptions

An option to process deactivation for open-unlinked items at the moment of last close.

static var forPreallocatedItems: FSVolume.ItemDeactivationOptions

An option to process deactivation for for files with preallocated space.

static var always: FSVolume.ItemDeactivationOptions

An option to always perform deactivation calls.

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

### Setting deactivation policy

var itemDeactivationPolicy: FSVolume.ItemDeactivationOptions

A property that tells FSKit to which types of items the deactivation applies, if any.

**Required**

