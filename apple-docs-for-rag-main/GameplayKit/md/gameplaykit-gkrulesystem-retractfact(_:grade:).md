

- GameplayKit
- GKRuleSystem
-  retractFact(\_:grade:) 

Instance Method

# retractFact(\_:grade:)

Reduces the membership grade of the specified fact by the specified amount, removing it from the fact set if necessary, and reevaluates the rules in the system’s agenda.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func retractFact(
    _ fact: any NSObjectProtocol,
    grade: Float
)
```

## Parameters 

`fact`  

An object representing a truth to be claimed or rejected by the rule system. For details, see the facts property.

`grade`  

The amount by which to reduce the fact’s membership grade.

## Discussion

Each fact has a membership grade ranging from zero to 1.0, representing variable levels of truth, strength, or confidence for use in fuzzy logic. Calling this method reduces the fact’s grade by the amount specified in the `grade` parameter; reducing a fact’s grade to zero or below removes it from the facts array.

Upon asserting or retracting any facts, the system reevaluates the rules in its agenda list so any rules that depend on changes to the set of facts can perform their actions.

## See Also

### Asserting and Retracting Facts

var facts: [Any]

The list of facts claimed by the rule system.

func assertFact(any NSObjectProtocol)

Adds the specified fact to the fact set with a membership grade of 1.0, and reevaluates the rules in the system’s agenda.

func assertFact(any NSObjectProtocol, grade: Float)

Increases the membership grade of the specified fact by the specified amount, adding it to the fact set if necessary, and reevaluates the rules in the system’s agenda.

func retractFact(any NSObjectProtocol)

Removes the specified fact from the fact set, and reevaluates the rules in the system’s agenda.

