

- Network Extension
- NEAppRule
-  matchSigningIdentifier 

Instance Property

# matchSigningIdentifier

The signing identifier of the app that matches the rule.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var matchSigningIdentifier: String { get }
```

## See Also

### Accessing app rule properties

var matchDesignatedRequirement: String

The designated requirement of the app that matches the rule.

var matchPath: String?

The file system path of the app that matches the rule.

var matchDomains: [Any]?

The hostname domains that match the rule.

var matchTools: [NEAppRule]?

An array of app rule objects that restrict the rule so it only matches network traffic generated from helper processes.

