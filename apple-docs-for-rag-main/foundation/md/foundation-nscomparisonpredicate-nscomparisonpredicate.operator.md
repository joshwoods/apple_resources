

- Foundation
- NSComparisonPredicate
-  NSComparisonPredicate.Operator 

Enumeration

# NSComparisonPredicate.Operator

Defines the type of comparison for a comparison predicate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Operator
```

## Topics

### Constants

case lessThan

A less-than predicate.

case lessThanOrEqualTo

A less-than-or-equal-to predicate.

case greaterThan

A greater-than predicate.

case greaterThanOrEqualTo

A greater-than-or-equal-to predicate.

case equalTo

An equal-to predicate.

case notEqualTo

A not-equal-to predicate.

case matches

A full regular expression matching predicate.

case like

A simple subset of the MATCHES predicate, similar in behavior to SQL `LIKE`.

case beginsWith

A begins-with predicate.

case endsWith

An ends-with predicate.

case `in`

A predicate to determine if the left hand side is in the right hand side.

case customSelector

A predicate that uses a custom selector that takes a single argument and returns a `BOOL` value.

case contains

A predicate to determine if the left hand side contains the right hand side.

case between

A predicate to determine if the left hand side lies at or between bounds specified by the right hand side.

case lessThan

A less-than predicate.

case lessThanOrEqualTo

A less-than-or-equal-to predicate.

case greaterThan

A greater-than predicate.

case greaterThanOrEqualTo

A greater-than-or-equal-to predicate.

case equalTo

An equal-to predicate.

case notEqualTo

A not-equal-to predicate.

case matches

A full regular expression matching predicate.

case like

A simple subset of the MATCHES predicate, similar in behavior to SQL `LIKE`.

case beginsWith

A begins-with predicate.

case endsWith

An ends-with predicate.

case `in`

A predicate to determine if the left hand side is in the right hand side.

case customSelector

A predicate that uses a custom selector that takes a single argument and returns a `BOOL` value.

case contains

A predicate to determine if the left hand side contains the right hand side.

case between

A predicate to determine if the left hand side lies at or between bounds specified by the right hand side.

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

### Getting Information About a Comparison Predicate

var comparisonPredicateModifier: NSComparisonPredicate.Modifier

The comparison predicate modifier for the receiver.

enum Modifier

Constants that describe the possible types of modifier for a comparison predicate.

var customSelector: Selector?

The selector for the receiver.

var rightExpression: NSExpression

The right expression for the receiver.

var leftExpression: NSExpression

The left expression for the receiver.

var options: NSComparisonPredicate.Options

The options to use for the receiver.

struct Options

Constants that describe the possible types of string comparison for comparison predicates.

var predicateOperatorType: NSComparisonPredicate.Operator

The predicate type for the receiver.

