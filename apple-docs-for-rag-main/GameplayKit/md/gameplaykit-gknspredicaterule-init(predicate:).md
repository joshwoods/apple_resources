

- GameplayKit
- GKNSPredicateRule
-  init(predicate:) 

Initializer

# init(predicate:)

Initializes a rule with the specified predicate.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(predicate: NSPredicate)
```

## Parameters 

`predicate`  

A predicate to be tested when evaluating the rule.

## Return Value

A new predicate-based rule object.

## Discussion

Rules based on NSPredicate objects typically test information in the state dictionary of the rule system evaluating the rule. For example, the following code creates a rule you might use to determine whether an enemy character in a game behaves aggressively.

- Swift
- Objective-C

```
// MyNSPredicateRule is a GKNSPredicateRule subclass
let healthTest = NSPredicate(format: "$player.health > 50")
let rule = MyNSPredicateRule(predicate: healthTest)
```

```
// MyNSPredicateRule is a GKNSPredicateRule subclass
NSPredicate *healthTest = [NSPredicate predicateWithFormat:@"$player.health > 50"];
MyNSPredicateRule *rule = [MyNSPredicateRule alloc] initWithPredicate:healthTest];
```

This example presumes the rule system’s state dictionary contains an object for the key `player`, which in turn exposes a numeric value for the key `health`. The GKNSPredicateRule class by itself does nothing in its performAction(in:) method—to create actions for predicate-based rules, you must subclass GKNSPredicateRule.

For more information, see GameplayKit Programming Guide.

