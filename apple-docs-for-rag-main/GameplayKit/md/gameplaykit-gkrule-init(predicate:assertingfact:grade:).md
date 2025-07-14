

- GameplayKit
- GKRule
-  init(predicate:assertingFact:grade:) 

Initializer

# init(predicate:assertingFact:grade:)

Creates a data-driven rule with the specified predicate, whose action asserts a fact in the rule system evaluating the rule.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    predicate: NSPredicate,
    assertingFact fact: any NSObjectProtocol,
    grade: Float
)
```

## Parameters 

`fact`  

An object representing a fact to assert when the rule’s predicate is satisfied. (For details on facts in rule systems, see the facts property in GKRuleSystem.)

`grade`  

An amount by which to increase the fact’s membership grade if the rule’s predicate is satisfied.

## Return Value

A new rule object.

## Discussion

Rules created using this method encode their predicate and action when archived with the NSKeyedArchiver class. You can use this feature to support saving and loading rules, editing rules in-game, or building tools that separate your gameplay design and game programming tasks.

Rules based on NSPredicate objects typically test information in the state dictionary of the rule system evaluating the rule. For example, the following code creates a rule you might use to determine whether an enemy character in a game behaves aggressively. (This example presumes the rule system’s state dictionary contains an object for the key `player`, which in turn exposes a numeric value for the key `health`.)

- Swift
- Objective-C

```
let healthTest = NSPredicate(format: "$player.health 

```
NSPredicate *healthTest = [NSPredicate predicateWithFormat:@"$player.health 

## See Also

### Creating Data-Driven Rules

convenience init(predicate: NSPredicate, retractingFact: any NSObjectProtocol, grade: Float)

Creates a data-driven rule with the specified predicate, whose action retracts a fact in the rule system evaluating the rule.

