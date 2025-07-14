

- GameplayKit
- GKAgentDelegate
-  agentDidUpdate(\_:) 

Instance Method

# agentDidUpdate(\_:)

Tells the delegate that an agent has just performed a simulation step.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
optional func agentDidUpdate(_ agent: GKAgent)
```

## Parameters 

`agent`  

The agent object that has just performed a simulation step.

## Discussion

Implement this method when you want to update a display based on the latest data from the agent simulation. Read the position and rotation properties of the agent (as a GKAgent2D or GKAgent3D object), then set the corresponding attributes of the object that provides the agent’s visual representation.

## See Also

### Synchronizing with Agents

func agentWillUpdate(GKAgent)

Tells the delegate that an agent is about to perform its next simulation step.

