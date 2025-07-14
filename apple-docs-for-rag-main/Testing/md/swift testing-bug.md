

- Swift Testing
-  Bug 

Structure

# Bug

A type representing a bug report tracked by a test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct Bug
```

## Mentioned in 

Interpreting bug identifiers

Adding comments to tests

## Overview

To add this trait to a test, use one of the following functions:

- bug(_:_:)

- bug(_:id:_:)

- bug(_:id:_:)

## Topics

### Instance Properties

var id: String?

A unique identifier in this bug’s associated bug-tracking system, if available.

var title: Comment?

The human-readable title of the bug, if specified by the test author.

var url: String?

A URL linking to more information about the bug, if available.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

SuiteTrait Implementations

Trait Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- SuiteTrait
- TestTrait
- Trait

## See Also

### Supporting types

struct Comment

A type representing a comment related to a test.

struct ConditionTrait

A type that defines a condition which must be satisfied for a test to be enabled.

struct ParallelizationTrait

A type that affects whether or not a test or suite is parallelized.

struct Tag

A type representing a tag that can be applied to a test.

struct List

A type representing one or more tags applied to a test.

struct TimeLimitTrait

A type that defines a time limit to apply to a test.

