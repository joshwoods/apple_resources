

- Foundation
- NSComparisonPredicate
-  NSComparisonPredicate.Modifier 

Enumeration

# NSComparisonPredicate.Modifier

Constants that describe the possible types of modifier for a comparison predicate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Modifier
```

## Topics

### Constants

case direct

A predicate to compare directly the left and right hand sides.

case all

A predicate to compare all entries in the destination of a to-many relationship.

case any

A predicate to match with any entry in the destination of a to-many relationship.

case direct

A predicate to compare directly the left and right hand sides.

case all

A predicate to compare all entries in the destination of a to-many relationship.

case any

A predicate to match with any entry in the destination of a to-many relationship.

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

enum Operator

Defines the type of comparison for a comparison predicate.

