

- SceneKit
- SCNActionable
-  actionKeys 

Instance Property

# actionKeys

The list of keys for which the node has attached actions.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var actionKeys: [String] { get }
```

**Required**

## Discussion

Use this property to list actions you scheduled using the runAction(_:forKey:) or runAction(_:forKey:completionHandler:) method.

## See Also

### Inspecting a Node’s Running Actions

func action(forKey: String) -> SCNAction?

Returns an action associated with a specific key.

**Required**

var hasActions: Bool

A Boolean value that indicates whether the node is currently executing any actions.

**Required**

