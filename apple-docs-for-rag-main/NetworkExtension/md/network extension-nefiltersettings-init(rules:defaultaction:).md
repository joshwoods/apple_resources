

- Network Extension
- NEFilterSettings
-  init(rules:defaultAction:) 

Initializer

# init(rules:defaultAction:)

Creates a new settings instance from an array of rules and a default action.

macOS 10.15+

``` source
init(
    rules: [NEFilterRule],
    defaultAction: NEFilterAction
)
```

## Parameters 

`rules`  

An array containing an ordered list of NEFilterRule objects. The maximum number of rules that this array can contain is 1000.

`defaultAction`  

The NEFilterAction to take for flows of network data that don’t match any of the specified rules. The default `defaultAction` is NEFilterAction.filterData. If `defaultAction` is NEFilterAction.allow or NEFilterAction.drop, then the `rules` array must contain at least one NEFilterRule.

## See Also

### Creating Filter Settings

class NEFilterRule

A rule for filters that combines a rule to match network traffic and an action to take when the rule matches.

