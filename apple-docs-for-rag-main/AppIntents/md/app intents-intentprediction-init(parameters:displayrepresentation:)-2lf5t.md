

- App Intents
- IntentPrediction
-  init(parameters:displayRepresentation:) 

Initializer

# init(parameters:displayRepresentation:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    parameters: T,
    displayRepresentation: @escaping (V0, V1, V2, V3, V4, V5, V6, V7, V8, V9, V10, V11, V12, V13, V14) -> DisplayRepresentation
) where T == (K0, K1, K2, K3, K4, K5, K6, K7, K8, K9, K10, K11, K12, K13, K14), V0 : _IntentValue, V0 : Sendable, V1 : _IntentValue, V1 : Sendable, V2 : _IntentValue, V2 : Sendable, V3 : _IntentValue, V3 : Sendable, V4 : _IntentValue, V4 : Sendable, V5 : _IntentValue, V5 : Sendable, V6 : _IntentValue, V6 : Sendable, V7 : _IntentValue, V7 : Sendable, V8 : _IntentValue, V8 : Sendable, V9 : _IntentValue, V9 : Sendable, V10 : _IntentValue, V10 : Sendable, V11 : _IntentValue, V11 : Sendable, V12 : _IntentValue, V12 : Sendable, V13 : _IntentValue, V13 : Sendable, V14 : _IntentValue, V14 : Sendable, P0 : IntentParameter, P1 : IntentParameter, P2 : IntentParameter, P3 : IntentParameter, P4 : IntentParameter, P5 : IntentParameter, P6 : IntentParameter, P7 : IntentParameter, P8 : IntentParameter, P9 : IntentParameter, P10 : IntentParameter, P11 : IntentParameter, P12 : IntentParameter, P13 : IntentParameter, P14 : IntentParameter, K0 : KeyPath, K1 : KeyPath, K2 : KeyPath, K3 : KeyPath, K4 : KeyPath, K5 : KeyPath, K6 : KeyPath, K7 : KeyPath, K8 : KeyPath, K9 : KeyPath, K10 : KeyPath, K11 : KeyPath, K12 : KeyPath, K13 : KeyPath, K14 : KeyPath
```

Available when `Intent` conforms to `AppIntent`.

