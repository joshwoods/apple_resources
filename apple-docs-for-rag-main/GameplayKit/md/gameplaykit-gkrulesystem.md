

- GameplayKit
-  GKRuleSystem 

Class

# GKRuleSystem

A list of rules, together with a context for evaluating them and interpreting results, for use in constructing data-driven logic or fuzzy logic systems.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKRuleSystem
```

## Overview

A GKRuleSystem object manages a list of rules (GKRule objects). A rule system also offers methods for evaluating its list of rules in a context defined by two features: a state dictionary containing information to be tested by rules, and a set of facts representing the conclusions drawn as a result of rule evaluation. You can evaluate facts based on a binary truth state—that is, a fact either is or is not in the set—or on a continuously variable membership grade, representing different levels of veracity, confidence, or strength for use in fuzzy logic.

You construct a rule system by creating GKRule objects and adding them to the system’s list of rules. There are multiple ways to construct rules: for greater reusability, use the methods listed in Creating Data-Driven Rules; or for greater flexibility, use the init(blockPredicate:action:) method or create a custom subclass of GKRule or GKNSPredicateRule. Then, add rules to the system with the methods listed in Managing a System’s List of Rules below.

To evaluate a system, call the evaluate() method. This method processes each rule in the system in the order it appears in the system’s agenda list. You set this order with the salience property of each rule, or with the order in which you add rules to the system. As the system processes each rule, it tests the rule’s evaluatePredicate(in:) method to determine whether the rule is satisfied in the context of the system. If the rule’s predicate is satisfied, the system executes the rule’s performAction(in:) method and moves the rule to the executed list (so the further evaluation of the agenda doesn’t repeatedly trigger the rule’s action).

Rules typically use the system’s state dictionary as input and its set of facts as output. (However, more complex systems can include sets of rules whose predicates test facts or whose actions mutate the system’s state.) After evaluating a rule system, you can examine the set of facts it has produced using the methods listed in Drawing Conclusions from Facts below. You can then use the presence of a fact in the set, the value of its membership grade, or the combined membership grades of a group of facts to influence the behaviors in your game.

For more information about rules and rule systems, read Rule Systems in GameplayKit Programming Guide.

## Topics

### Creating a Rule System

init()

Initializes a new, empty rule system.

### Managing State Information

var state: NSMutableDictionary

A dictionary of state information to be evaluated by the system’s rules.

### Managing a System’s List of Rules

var rules: [GKRule]

The list of rules to be executed when evaluating the system.

func add(GKRule)

Adds the specified rule to the system.

func add([GKRule])

Adds the specified list of rules to the system.

func removeAllRules()

Removes all rules from the system.

### Evaluating a Rule System

func evaluate()

Evaluates the rule system, executing the list of rules in its agenda.

var agenda: [GKRule]

The list of rules to be considered when evaluating the system.

var executed: [GKRule]

The list of rules whose actions have been performed during evaluation of the system.

func reset()

Returns the rule system to its original agenda and clears all facts.

### Asserting and Retracting Facts

var facts: [Any]

The list of facts claimed by the rule system.

func assertFact(any NSObjectProtocol)

Adds the specified fact to the fact set with a membership grade of 1.0, and reevaluates the rules in the system’s agenda.

func assertFact(any NSObjectProtocol, grade: Float)

Increases the membership grade of the specified fact by the specified amount, adding it to the fact set if necessary, and reevaluates the rules in the system’s agenda.

func retractFact(any NSObjectProtocol)

Removes the specified fact from the fact set, and reevaluates the rules in the system’s agenda.

func retractFact(any NSObjectProtocol, grade: Float)

Reduces the membership grade of the specified fact by the specified amount, removing it from the fact set if necessary, and reevaluates the rules in the system’s agenda.

### Drawing Conclusions from Facts

func grade(forFact: any NSObjectProtocol) -> Float

Returns the membership grade of the specified fact.

func minimumGrade(forFacts: [Any]) -> Float

Returns the lowest membership grade among the specified facts.

func maximumGrade(forFacts: [Any]) -> Float

Returns the highest membership grade among the specified facts.

## Relationships

### Inherits From

- NSObject

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

class GKNSPredicateRule

A rule for use in a rule system that uses a Foundation NSPredicate object to evaluate itself.

