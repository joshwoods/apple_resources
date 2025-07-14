

- GameplayKit
- GKRuleSystem
-  removeAllRules() 

Instance Method

# removeAllRules()

Removes all rules from the system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func removeAllRules()
```

## Discussion

Calling this method also empties the agenda and executed arrays.

## See Also

### Related Documentation

var agenda: [GKRule]

The list of rules to be considered when evaluating the system.

var executed: [GKRule]

The list of rules whose actions have been performed during evaluation of the system.

### Managing a System’s List of Rules

var rules: [GKRule]

The list of rules to be executed when evaluating the system.

func add(GKRule)

Adds the specified rule to the system.

func add([GKRule])

Adds the specified list of rules to the system.

