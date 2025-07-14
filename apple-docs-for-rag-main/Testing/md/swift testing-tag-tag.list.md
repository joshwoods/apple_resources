

- Swift Testing
- Tag
-  Tag.List 

Structure

# Tag.List

A type representing one or more tags applied to a test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct List
```

## Overview

To add this trait to a test, use the tags(_:) function.

## Topics

### Instance Properties

var tags: [Tag]

The list of tags contained in this instance.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

SuiteTrait Implementations

Trait Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable
- SuiteTrait
- TestTrait
- Trait

## See Also

### Supporting types

struct Bug

A type representing a bug report tracked by a test.

struct Comment

A type representing a comment related to a test.

struct ConditionTrait

A type that defines a condition which must be satisfied for a test to be enabled.

struct ParallelizationTrait

A type that affects whether or not a test or suite is parallelized.

struct Tag

A type representing a tag that can be applied to a test.

struct TimeLimitTrait

A type that defines a time limit to apply to a test.

