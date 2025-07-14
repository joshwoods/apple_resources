

- GameplayKit
-  GKNSPredicateRule 

Class

# GKNSPredicateRule

A rule for use in a rule system that uses a Foundation NSPredicate object to evaluate itself.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKNSPredicateRule
```

## Overview

The GKNSPredicateRule class is a specialized subclass of the GKRule class (which represents rules to be used by GKRuleSystem objects). Custom subclasses of GKNSPredicateRule use an NSPredicate object to evaluate a rule, rather than requiring custom logic for evaluation as is the case with custom GKRule subclasses.

For more information about rules and rule systems, read Rule Systems in GameplayKit Programming Guide.

### Subclassing Notes

GameplayKit evaluates rules in the context of a GKRuleSystem object, so custom rule classes should be *functional*—that is, they generally should not carry independent state that affects their predicate or action.

#### Methods to Override

Override the performAction(in:) method to perform whatever actions should result when your rule is satisfied (that is, when its predicate property evaluates to true in the context of the provided rule system).

#### Alternatives to Subclassing

- Use the GKRule method init(predicate:assertingFact:grade:) or init(predicate:retractingFact:grade:) to create a rule that uses an NSPredicate object for evaluation and whose action asserts or retracts a fact in the containing rule system.

- Use the GKRule method init(blockPredicate:action:) method to quickly create a rule whose custom logic is contained in block objects.

## Topics

### Creating a Predicate-Based Rule

init(predicate: NSPredicate)

Initializes a rule with the specified predicate.

### Evaluating a Rule

var predicate: NSPredicate

A predicate to be tested when evaluating the rule.

func evaluatePredicate(in: GKRuleSystem) -> Bool

Returns a Boolean value indicating whether the rule’s predicate has been satisfied in the context of the specified rule system.

## Relationships

### Inherits From

- GKRule

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Rule Systems

class GKRule

A rule to be used in the context of a rule system, with a predicate to be tested and an action to be executed when the test succeeds.

class GKRuleSystem

A list of rules, together with a context for evaluating them and interpreting results, for use in constructing data-driven logic or fuzzy logic systems.

