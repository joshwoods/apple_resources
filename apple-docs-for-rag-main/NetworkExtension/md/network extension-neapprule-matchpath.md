

- Network Extension
- NEAppRule
-  matchPath 

Instance Property

# matchPath

The file system path of the app that matches the rule.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var matchPath: String? { get set }
```

## See Also

### Accessing app rule properties

var matchSigningIdentifier: String

The signing identifier of the app that matches the rule.

var matchDesignatedRequirement: String

The designated requirement of the app that matches the rule.

var matchDomains: [Any]?

The hostname domains that match the rule.

var matchTools: [NEAppRule]?

An array of app rule objects that restrict the rule so it only matches network traffic generated from helper processes.

