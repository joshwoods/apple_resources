

- SceneKit
- SCNActionable
-  hasActions 

Instance Property

# hasActions

A Boolean value that indicates whether the node is currently executing any actions.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var hasActions: Bool { get }
```

**Required**

## Discussion

This value is true if the node has any executing actions; otherwise the value is false.

## See Also

### Inspecting a Node’s Running Actions

func action(forKey: String) -> SCNAction?

Returns an action associated with a specific key.

**Required**

var actionKeys: [String]

The list of keys for which the node has attached actions.

**Required**

