

- Swift Testing
-  Comment 

Structure

# Comment

A type representing a comment related to a test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct Comment
```

## Overview

This type may be used to provide context or background information about a test’s purpose, explain how a complex test operates, or include details which may be helpful when diagnosing issues recorded by a test.

To add a comment to a test or suite, add a code comment before its `@Test` or `@Suite` attribute. See Adding comments to tests for more details.

Note

This type is not intended to reference bugs related to a test. Instead, use bug(_:_:), bug(_:id:_:), or bug(_:id:_:).

## Topics

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

The single comment string contained in this instance.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringInterpolation Implementations

ExpressibleByStringLiteral Implementations

ExpressibleByUnicodeScalarLiteral Implementations

RawRepresentable Implementations

SuiteTrait Implementations

Trait Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- RawRepresentable
- Sendable
- SuiteTrait
- TestTrait
- Trait

## See Also

### Supporting types

struct Bug

A type representing a bug report tracked by a test.

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

