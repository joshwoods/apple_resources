

- GameplayKit
- GKRuleSystem
-  facts 

Instance Property

# facts

The list of facts claimed by the rule system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var facts: [Any] { get }
```

## Discussion

A fact is any object representing a truth claimed by the rule system. You can use any type of object to represent the facts in your system: simple data types like strings and numbers typically suffice, but you can also use custom objects from your game’s data model.

Each fact has a membership grade ranging from zero to 1.0, representing variable levels of truth, strength, or confidence for use in fuzzy logic. Asserting a fact increases its grade, adding it to the array if not present; retracting a set reduces its grade, removing it from the array if its grade drops to zero. Use the GKRuleSystem methods listed in Drawing Conclusions from Facts to examine the grade of a fact or of a combination of facts.

## See Also

### Asserting and Retracting Facts

func assertFact(any NSObjectProtocol)

Adds the specified fact to the fact set with a membership grade of 1.0, and reevaluates the rules in the system’s agenda.

func assertFact(any NSObjectProtocol, grade: Float)

Increases the membership grade of the specified fact by the specified amount, adding it to the fact set if necessary, and reevaluates the rules in the system’s agenda.

func retractFact(any NSObjectProtocol)

Removes the specified fact from the fact set, and reevaluates the rules in the system’s agenda.

func retractFact(any NSObjectProtocol, grade: Float)

Reduces the membership grade of the specified fact by the specified amount, removing it from the fact set if necessary, and reevaluates the rules in the system’s agenda.

