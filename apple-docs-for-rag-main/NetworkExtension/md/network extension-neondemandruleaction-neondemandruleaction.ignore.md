

- Network Extension
- NEOnDemandRuleAction
-  NEOnDemandRuleAction.ignore 

Case

# NEOnDemandRuleAction.ignore

Do not start the VPN connection, but do not disconnect it if it is currently connected.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
case ignore
```

## See Also

### Rule Actions

case connect

Start the VPN connection for every connection attempt.

case disconnect

Do not start the VPN connection, and disconnect the VPN connection if it is not currently disconnected.

case evaluateConnection

Start the VPN after evaluating the destination host being accessed against the rule’s parameters.

