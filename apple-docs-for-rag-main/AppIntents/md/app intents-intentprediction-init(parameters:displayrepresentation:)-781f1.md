

- App Intents
- IntentPrediction
-  init(parameters:displayRepresentation:) 

Initializer

# init(parameters:displayRepresentation:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    parameters: T,
    displayRepresentation: @escaping (V0, V1, V2, V3, V4, V5, V6, V7) -> DisplayRepresentation
) where T == (K0, K1, K2, K3, K4, K5, K6, K7), V0 : _IntentValue, V0 : Sendable, V1 : _IntentValue, V1 : Sendable, V2 : _IntentValue, V2 : Sendable, V3 : _IntentValue, V3 : Sendable, V4 : _IntentValue, V4 : Sendable, V5 : _IntentValue, V5 : Sendable, V6 : _IntentValue, V6 : Sendable, V7 : _IntentValue, V7 : Sendable, P0 : IntentParameter, P1 : IntentParameter, P2 : IntentParameter, P3 : IntentParameter, P4 : IntentParameter, P5 : IntentParameter, P6 : IntentParameter, P7 : IntentParameter, K0 : KeyPath, K1 : KeyPath, K2 : KeyPath, K3 : KeyPath, K4 : KeyPath, K5 : KeyPath, K6 : KeyPath, K7 : KeyPath
```

Available when `Intent` conforms to `AppIntent`.

