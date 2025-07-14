

- Foundation
- NSComparisonPredicate
-  predicateOperatorType 

Instance Property

# predicateOperatorType

The predicate type for the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var predicateOperatorType: NSComparisonPredicate.Operator { get }
```

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

enum Operator

Defines the type of comparison for a comparison predicate.

