

- SpriteKit
- SKAction
-  reversed() 

Instance Method

# reversed()

Creates an action that reverses the behavior of another action.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func reversed() -> SKAction
```

## Return Value

A new action that reverses an action’s behavior.

## Mentioned in 

Getting Started with Actions

## Discussion

This method always returns an action object; however, not all actions are reversible. When reversed, some actions return an object that either does nothing or that performs the same action as the original action. For details on how an action is reversed, see the description of the class method used to create that action.

