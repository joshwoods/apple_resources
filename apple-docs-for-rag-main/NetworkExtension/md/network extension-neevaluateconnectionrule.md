

- Network Extension
-  NEEvaluateConnectionRule 

Class

# NEEvaluateConnectionRule

`NEEvaluateConnectionRule` associates properties of network connections with an action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEEvaluateConnectionRule
```

## Topics

### Initializing a Rule

init(matchDomains: [String], andAction: NEEvaluateConnectionRuleAction)

Initialize an `NEEvaluateConnectionRule` instance with a list of destination host domains and an action.

### Accessing Rule Match Properties

var matchDomains: [String]

An array of domains used to match the destination hostname of connections. If the destination hostname of a connection matches any of the domains in the array, then the connection matches the rule. Each domain is matched against the destination hostname using suffix matching, and each label in the domain must match an entire label in the hostname. For example, the domain `example.com` will match the hostname `www.example.com` but not `www.anotherexample.com`.

var useDNSServers: [String]?

If the rule matches the connection being established and the action is `NEEvaluateConnectionRuleActionConnectIfNeeded`, the DNS servers specified in this array are used to resolve the destination hostname of the connection while evaluating connectivity to the destination of the connection. If the resolution fails for any reason, the VPN is started.

var probeURL: URL?

An HTTP or HTTPS URL. If the rule matches the connection being established and the action is `NEEvaluateConnectionRuleActionConnectIfNeeded` and a request sent to this URL results in a response with an HTTP response code other than 200, then the VPN is started.

### Accessing the Rule Action

var action: NEEvaluateConnectionRuleAction

The action to take if the properties of the network connection being established match the rule.

enum NEEvaluateConnectionRuleAction

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Accessing connection rules

var connectionRules: [NEEvaluateConnectionRule]?

An array of NEEvaluateConnectionRule objects

