

- GameplayKit
- GKRule
-  performAction(in:) 

Instance Method

# performAction(in:)

Performs actions that should result when the rule is satisfied in the context of the specified rule system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func performAction(in system: GKRuleSystem)
```

## Discussion

A rule system calls this method when evaluating its rules, if and only if the rule’s predicate has been satisfied (that is, the evaluatePredicate(in:) method has returned true), and after moving the rule from its agenda list to its executed list.

If the rule was created with the init(predicate:assertingFact:grade:) or init(predicate:retractingFact:grade:), calling this method asserts or retracts the fact as specified in the provided rule system. If the rule was created with the init(blockPredicate:action:) method, calling this method calls the action block. Otherwise, this method does nothing—subclasses should override this method to implement their own actions.

## See Also

### Evaluating a Rule

func evaluatePredicate(in: GKRuleSystem) -> Bool

Returns a Boolean value indicating whether the rule has been satisfied in the context of the specified rule system.

