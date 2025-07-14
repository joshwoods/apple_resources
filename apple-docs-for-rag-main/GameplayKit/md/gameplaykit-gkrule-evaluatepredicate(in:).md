

- GameplayKit
- GKRule
-  evaluatePredicate(in:) 

Instance Method

# evaluatePredicate(in:)

Returns a Boolean value indicating whether the rule has been satisfied in the context of the specified rule system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func evaluatePredicate(in system: GKRuleSystem) -> Bool
```

## Return Value

true if the rule is satisfied (and its action should be executed); otherwise, false.

## Discussion

A rule system calls this method when evaluating its rules.

If the rule was created with the init(predicate:assertingFact:grade:) or init(predicate:retractingFact:grade:), calling this method returns the result of testing the predicate against the provided rule system. If the rule was created with the init(blockPredicate:action:) method, calling this method calls the predicate block and returns the result. Otherwise, this method always returns false—subclasses should override this method to implement their own predicate tests.

## See Also

### Evaluating a Rule

func performAction(in: GKRuleSystem)

Performs actions that should result when the rule is satisfied in the context of the specified rule system.

