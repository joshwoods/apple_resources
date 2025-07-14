

- Device Management
- ServiceManagementManagedLoginItems
-  ServiceManagementManagedLoginItems.Rule 

Device Management Profile

# ServiceManagementManagedLoginItems.Rule

A dictionary that configures a service management rule.

macOS 13.0+Device Assignment ServicesVPP License Management

``` source
object ServiceManagementManagedLoginItems.Rule
```

## Properties

`Comment`

`string`

An optional description of the rule.

`RuleType`

`string`

 (Required) 

The type of comparison to make.

Possible Values: `BundleIdentifier, BundleIdentifierPrefix, Label, LabelPrefix, TeamIdentifier`

`RuleValue`

`string`

 (Required) 

The value to compare with each login item’s value, to determine if this rule is a match.

`TeamIdentifier`

`string`

An additional constraint to limit the scope of the rule that the system tests after matching the `RuleType` and `RuleValue`.

