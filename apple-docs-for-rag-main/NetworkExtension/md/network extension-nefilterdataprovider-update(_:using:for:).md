

- Network Extension
- NEFilterDataProvider
-  update(\_:using:for:) 

Instance Method

# update(\_:using:for:)

Updates the verdict for a flow outside the context of any filter data provider callback.

macOS 10.15.4+

``` source
func update(
    _ flow: NEFilterSocketFlow,
    using verdict: NEFilterDataVerdict,
    for direction: NETrafficDirection
)
```

## Parameters 

`flow`  

The NEFilterSocketFlow to update the verdict for.

`verdict`  

An NEFilterDataVerdict instance. This must be an allow() or drop() verdict, or a data verdict created with the Swift initializer or ObjectiveC type method, init(passBytes:peekBytes:).

`direction`  

The direction to which the verdict applies. Pass NETrafficDirection.any to update the verdict for both the inbound and outbound directions. This parameter has no effect if the verdict is drop().

