

- GameplayKit
- GKRuleSystem
-  add(\_:) 

Instance Method

# add(\_:)

Adds the specified list of rules to the system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func add(_ rules: [GKRule])
```

## Parameters 

`rules`  

An array of rule objects.

## Discussion

Adding rules to the system also adds them to the agenda list, in decreasing order of the rules’ salience values. Rules with the same salience are added to the agenda in the order of the specified array.

## See Also

### Related Documentation

var agenda: [GKRule]

The list of rules to be considered when evaluating the system.

### Managing a System’s List of Rules

var rules: [GKRule]

The list of rules to be executed when evaluating the system.

func add(GKRule)

Adds the specified rule to the system.

func removeAllRules()

Removes all rules from the system.

