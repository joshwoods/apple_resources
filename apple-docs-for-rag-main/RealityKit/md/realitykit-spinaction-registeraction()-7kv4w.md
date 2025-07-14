

- RealityKit
- SpinAction
-  registerAction() 

Type Method

# registerAction()

Registers the serializable action into the action-types registry.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func registerAction()
```

Available when `Self` conforms to `Decodable`, `Self` conforms to `Encodable`, `EventParameterType` conforms to `Decodable`, and `EventParameterType` conforms to `Encodable`.

## Discussion

Registering an action allows RealityKit to retrieve its AnimationResource definitions.

Registering an action may not be necessary, because RealityKit automatically registers the action when you:

- Initialize an ActionAnimation with this action.

- Subscribe to it in any way, including subscribing an ActionHandlerProtocol.

