

- GameplayKit
- GKNSPredicateRule
-  evaluatePredicate(in:) 

Instance Method

# evaluatePredicate(in:)

Returns a Boolean value indicating whether the rule’s predicate has been satisfied in the context of the specified rule system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func evaluatePredicate(in system: GKRuleSystem) -> Bool
```

## Return Value

true if the rule is satisfied (and its action should be executed); otherwise, false.

## Discussion

The GKNSPredicateRule class overrides this method to use its predicate property for testing the rule. Subclasses of GKNSPredicateRule do not need to override this method.

## See Also

### Evaluating a Rule

var predicate: NSPredicate

A predicate to be tested when evaluating the rule.

