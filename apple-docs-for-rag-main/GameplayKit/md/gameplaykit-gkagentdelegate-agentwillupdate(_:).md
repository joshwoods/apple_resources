

- GameplayKit
- GKAgentDelegate
-  agentWillUpdate(\_:) 

Instance Method

# agentWillUpdate(\_:)

Tells the delegate that an agent is about to perform its next simulation step.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
optional func agentWillUpdate(_ agent: GKAgent)
```

## Parameters 

`agent`  

The agent object that will perform its next simulation step.

## Discussion

Implement this method when you want to update the agent simulation with data from an external source, such as node position and orientation information updated by the SceneKit or SpriteKit physics engine. Set the position and rotation properties of the agent (as a GKAgent2D or GKAgent3D object) so that the next simulation step will take your changes to those properties into account.

For more information, see GameplayKit Programming Guide.

## See Also

### Synchronizing with Agents

func agentDidUpdate(GKAgent)

Tells the delegate that an agent has just performed a simulation step.

