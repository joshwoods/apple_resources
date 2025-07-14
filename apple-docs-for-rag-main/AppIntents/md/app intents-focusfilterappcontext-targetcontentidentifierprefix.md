

- App Intents
- FocusFilterAppContext
-  targetContentIdentifierPrefix 

Instance Property

# targetContentIdentifierPrefix

An identifier you provide to the system for use in scheme prefixes for Focus.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
let targetContentIdentifierPrefix: String?
```

## Discussion

The system combines this prefix with the scheme `focus:` to prefix any `targetContentIdentifier` strings you provide for the system to evaluate against your app’s `sceneActivationConditions`.

