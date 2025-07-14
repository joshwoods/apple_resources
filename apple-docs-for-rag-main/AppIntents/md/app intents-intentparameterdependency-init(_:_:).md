

- App Intents
- IntentParameterDependency
-  init(\_:\_:) 

Initializer

# init(\_:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
convenience init(
    _ k0: KeyPath,
    _ k1: KeyPath
) where V0 : _IntentValue, V0 : Sendable, P0 : IntentParameter, V1 : _IntentValue, V1 : Sendable, P1 : IntentParameter
```

Available when `Intent` conforms to `AppIntent`.

