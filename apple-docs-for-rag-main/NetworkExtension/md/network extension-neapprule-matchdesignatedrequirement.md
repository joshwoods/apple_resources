

- Network Extension
- NEAppRule
-  matchDesignatedRequirement 

Instance Property

# matchDesignatedRequirement

The designated requirement of the app that matches the rule.

macOS 10.11+

``` source
var matchDesignatedRequirement: String { get }
```

## See Also

### Accessing app rule properties

var matchSigningIdentifier: String

The signing identifier of the app that matches the rule.

var matchPath: String?

The file system path of the app that matches the rule.

var matchDomains: [Any]?

The hostname domains that match the rule.

var matchTools: [NEAppRule]?

An array of app rule objects that restrict the rule so it only matches network traffic generated from helper processes.

