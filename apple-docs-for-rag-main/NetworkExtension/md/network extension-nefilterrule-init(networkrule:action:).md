

- Network Extension
- NEFilterRule
-  init(networkRule:action:) 

Initializer

# init(networkRule:action:)

Creates a new filter rule from a network rule and an action to take when network traffic matches.

macOS 10.15+

``` source
init(
    networkRule: NENetworkRule,
    action: NEFilterAction
)
```

## Parameters 

`networkRule`  

An NENetworkRule object that defines the network traffic characteristics that this rule matches.

`action`  

The action to take when the network rule matches.

