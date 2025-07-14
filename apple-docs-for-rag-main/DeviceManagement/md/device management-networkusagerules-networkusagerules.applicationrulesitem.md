

- Device Management
- NetworkUsageRules
-  NetworkUsageRules.ApplicationRulesItem 

Device Management Profile

# NetworkUsageRules.ApplicationRulesItem

The application rules dictionary.

iOS 9.0+iPadOS 9.0+Device Assignment ServicesVPP License Management

``` source
object NetworkUsageRules.ApplicationRulesItem
```

## Properties

`AllowCellularData`

`boolean`

If `false`, disables cellular data for all matching managed apps.

Default: `true`

`AllowRoamingCellularData`

`boolean`

If `false`, disables cellular data while roaming for all matching managed apps.

Default: `true`

`AppIdentifierMatches`

`[string]`

A list of managed app identifiers, as strings, that must follow the associated rules. If this key is missing, the rules apply to all managed apps on the device.

Each string in the `AppIdentifierMatches` array may either be an exact app identifier match (for example, `com.mycompany.myapp`) or it may specify a prefix match for the bundle ID by using the \* wildcard character. If used, this character must appear after a period (.) and may only appear once, at the end of the string; for example, `com.mycompany.*`.

## See Also

### Objects

object NetworkUsageRules.SIMRulesItem

The policy for individual SIM cards.

