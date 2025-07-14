

- Foundation
- NSCompoundPredicate
-  NSCompoundPredicate.LogicalType 

Enumeration

# NSCompoundPredicate.LogicalType

Constants that describe the possible types of a compound predicate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum LogicalType
```

## Topics

### Constants

case not

A logical NOT predicate.

case and

A logical AND predicate.

case or

A logical OR predicate.

case not

A logical NOT predicate.

case and

A logical AND predicate.

case or

A logical OR predicate.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Information About a Compound Predicate

var compoundPredicateType: NSCompoundPredicate.LogicalType

The predicate type for the receiver.

var subpredicates: [Any]

The receiver’s subpredicates.

