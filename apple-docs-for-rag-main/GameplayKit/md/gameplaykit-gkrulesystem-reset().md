

- GameplayKit
- GKRuleSystem
-  reset() 

Instance Method

# reset()

Returns the rule system to its original agenda and clears all facts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func reset()
```

## Discussion

Calling this method restarts the evaluation process: the system removes all rules from the current agenda and executed lists and empties the facts set. (However, the rule’s state dictionary is left unchanged.) The system then automatically repopulates its agenda according to the salience of each rule in the rules array.

## See Also

### Evaluating a Rule System

func evaluate()

Evaluates the rule system, executing the list of rules in its agenda.

var agenda: [GKRule]

The list of rules to be considered when evaluating the system.

var executed: [GKRule]

The list of rules whose actions have been performed during evaluation of the system.

