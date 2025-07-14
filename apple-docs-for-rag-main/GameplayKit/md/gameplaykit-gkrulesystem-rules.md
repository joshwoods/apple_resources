

- GameplayKit
- GKRuleSystem
-  rules 

Instance Property

# rules

The list of rules to be executed when evaluating the system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var rules: [GKRule] { get }
```

## Discussion

This array holds all rules under consideration by the system—that is, the union of the agenda and executed lists. The agenda holds the rules to be considered when evaluating the system, listed in order of their salience values (or, for rules with the same salience, the order in which they were added to the system). During evaluation of the rule system, if a rule on the agenda list is satisfied (that is, its predicate returns true and it executes its action) the system moves that rule to the executed list.

Changing the salience of a rule already in the rule system does not adjust its position in the agenda, but does determine the order of the new agenda when resetting the system.

## See Also

### Related Documentation

func reset()

Returns the rule system to its original agenda and clears all facts.

var agenda: [GKRule]

The list of rules to be considered when evaluating the system.

func evaluate()

Evaluates the rule system, executing the list of rules in its agenda.

var executed: [GKRule]

The list of rules whose actions have been performed during evaluation of the system.

### Managing a System’s List of Rules

func add(GKRule)

Adds the specified rule to the system.

func add([GKRule])

Adds the specified list of rules to the system.

func removeAllRules()

Removes all rules from the system.

