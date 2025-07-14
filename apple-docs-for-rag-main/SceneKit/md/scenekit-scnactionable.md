

- SceneKit
-  SCNActionable 

Protocol

# SCNActionable

Methods for running actions on nodes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol SCNActionable : NSObjectProtocol
```

## Overview

SCNAction objects represent reusable, animated actions that can be performed on nodes, such as moving or rotating them. You use an SCNAction class method to create an action and then use methods in the SCNActionable protocol to run the action on a node. This protocol also defines methods for checking whether a node has any currently running actions and, if so, canceling them.

## Topics

### Running Actions

func runAction(SCNAction)

Adds an action to the list of actions executed by the node.

**Required**

func runAction(SCNAction, completionHandler: (() -> Void)?)

Adds an action to the list of actions executed by the node. SceneKit calls the specified block when the action completes.

**Required**

func runAction(SCNAction, forKey: String?)

Adds an identifiable action to the list of actions executed by the node.

**Required**

func runAction(SCNAction, forKey: String?, completionHandler: (() -> Void)?)

Adds an identifiable action to the list of actions executed by the node. SceneKit calls the specified block when the action completes.

**Required**

### Inspecting a Node’s Running Actions

func action(forKey: String) -> SCNAction?

Returns an action associated with a specific key.

**Required**

var hasActions: Bool

A Boolean value that indicates whether the node is currently executing any actions.

**Required**

var actionKeys: [String]

The list of keys for which the node has attached actions.

**Required**

### Canceling a Node’s Running Actions

func removeAction(forKey: String)

Removes an action associated with a specific key.

**Required**

func removeAllActions()

Ends and removes all actions from the node.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SCNNode
- SCNReferenceNode

## See Also

### Actions

class SCNAction

A simple, reusable animation that changes attributes of any node you attach it to.

