

- Network Extension
- NEAppRule
-  matchDomains 

Instance Property

# matchDomains

The hostname domains that match the rule.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var matchDomains: [Any]? { get set }
```

## Discussion

If this property is set to a nonempty array, then only connections to destinations in the domains specified in the array will use the VPN.

## See Also

### Accessing app rule properties

var matchSigningIdentifier: String

The signing identifier of the app that matches the rule.

var matchDesignatedRequirement: String

The designated requirement of the app that matches the rule.

var matchPath: String?

The file system path of the app that matches the rule.

var matchTools: [NEAppRule]?

An array of app rule objects that restrict the rule so it only matches network traffic generated from helper processes.

