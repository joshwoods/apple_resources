

- Network Extension
- NEFilterSettings
-  rules 

Instance Property

# rules

An ordered list of rules that define the filter’s operation.

macOS 10.15+

``` source
var rules: [NEFilterRule] { get }
```

## Discussion

After applying the NEFilterSettings, the system compares each network flow against these rules in order, and acts on the rule of the first NEFilterAction that matches.

## See Also

### Inspecting Filter Settings

var defaultAction: NEFilterAction

The default action to take for flows of network data that don’t match any of the specified rules.

