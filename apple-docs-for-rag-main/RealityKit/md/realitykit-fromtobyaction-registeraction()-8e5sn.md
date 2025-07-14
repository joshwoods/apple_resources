

- RealityKit
- FromToByAction
-  registerAction() 

Type Method

# registerAction()

Registers the action into the action-types registry.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func registerAction()
```

## Discussion

Registering an action allows RealityKit to retrieve its AnimationResource definitions.

Registering an action may not be necessary, because RealityKit automatically registers the action when you:

- Initialize an ActionAnimation with this action.

- Subscribe to it in any way, including subscribing an ActionHandlerProtocol.

