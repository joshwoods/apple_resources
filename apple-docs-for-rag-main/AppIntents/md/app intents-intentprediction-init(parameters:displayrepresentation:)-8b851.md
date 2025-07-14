

- App Intents
- IntentPrediction
-  init(parameters:displayRepresentation:) 

Initializer

# init(parameters:displayRepresentation:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    parameters: T,
    displayRepresentation: @escaping (V0, V1, V2) -> DisplayRepresentation
) where T == (K0, K1, K2), V0 : _IntentValue, V0 : Sendable, V1 : _IntentValue, V1 : Sendable, V2 : _IntentValue, V2 : Sendable, P0 : IntentParameter, P1 : IntentParameter, P2 : IntentParameter, K0 : KeyPath, K1 : KeyPath, K2 : KeyPath
```

Available when `Intent` conforms to `AppIntent`.

