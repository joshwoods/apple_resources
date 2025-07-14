

- App Intents
- IntentPrediction
-  init(parameters:displayRepresentation:) 

Initializer

# init(parameters:displayRepresentation:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    parameters: T,
    displayRepresentation: @escaping (V0) -> DisplayRepresentation
) where T == KeyPath, V0 : _IntentValue, V0 : Sendable, P0 : IntentParameter
```

Available when `Intent` conforms to `AppIntent`.

