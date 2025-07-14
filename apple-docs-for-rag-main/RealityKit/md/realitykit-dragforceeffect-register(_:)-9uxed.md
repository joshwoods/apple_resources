

- RealityKit
- DragForceEffect
-  register(\_:) 

Type Method

# register(\_:)

Register the codable custom effect. If a handler is specified, the closure is used to update the effect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
static func register(_ updateHandler: (@MainActor (inout ForceEffectEvent) -> Void)? = nil)
```

Available when `Self` conforms to `Decodable` and `Encodable`.

