

- GameplayKit
- GKRuleSystem
-  add(\_:) 

Instance Method

# add(\_:)

Adds the specified rule to the system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func add(_ rule: GKRule)
```

## Parameters 

`rule`  

A rule object.

## Discussion

Adding rules to the system also adds them to the agenda list, in decreasing order of the rules’ salience values. Rules with the same salience are listed in the agenda in the order in which they were added to the system.

## See Also

### Related Documentation

var agenda: [GKRule]

The list of rules to be considered when evaluating the system.

### Managing a System’s List of Rules

var rules: [GKRule]

The list of rules to be executed when evaluating the system.

func add([GKRule])

Adds the specified list of rules to the system.

func removeAllRules()

Removes all rules from the system.

