

- SceneKit
- SCNActionable
-  action(forKey:) 

Instance Method

# action(forKey:)

Returns an action associated with a specific key.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func action(forKey key: String) -> SCNAction?
```

**Required**

## Parameters 

`key`  

A string that uniquely identifies a action.

## Return Value

The action object matching the specified key, or `nil` if the node does not have an action identified by the key.

## Discussion

Use this method to retrieve actions you scheduled using the runAction(_:forKey:) or runAction(_:forKey:completionHandler:) method.

## See Also

### Inspecting a Node’s Running Actions

var hasActions: Bool

A Boolean value that indicates whether the node is currently executing any actions.

**Required**

var actionKeys: [String]

The list of keys for which the node has attached actions.

**Required**

