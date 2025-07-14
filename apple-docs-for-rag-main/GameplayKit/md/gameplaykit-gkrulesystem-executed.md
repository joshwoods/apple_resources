

- GameplayKit
- GKRuleSystem
-  executed 

Instance Property

# executed

The list of rules whose actions have been performed during evaluation of the system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var executed: [GKRule] { get }
```

## Discussion

When you call the evaluate() method, the system considers each rule in the agenda list in order. If a rule on the agenda is satisfied—that is, its predicate returns true and it executes its action—the system moves that rule to the executed list.

## See Also

### Related Documentation

var rules: [GKRule]

The list of rules to be executed when evaluating the system.

### Evaluating a Rule System

func evaluate()

Evaluates the rule system, executing the list of rules in its agenda.

var agenda: [GKRule]

The list of rules to be considered when evaluating the system.

func reset()

Returns the rule system to its original agenda and clears all facts.

