

- App Intents
- AppShortcut
-  init(intent:phrases:shortTitle:systemImageName:parameterPresentation:) 

Initializer

# init(intent:phrases:shortTitle:systemImageName:parameterPresentation:)

Initializes an App Shortcut with phrases that run the app intent, a title, an image, and specified parameters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    intent: Intent,
    phrases: [AppShortcutPhrase],
    shortTitle: LocalizedStringResource,
    systemImageName: String,
    parameterPresentation: AppShortcutParameterPresentation
) where Intent : AppIntent, Value : _IntentValue, Value : Sendable, Parameter : IntentParameter, ParameterKeyPath : KeyPath
```

## Parameters 

`intent`  

The `AppIntent` associated with the `AppShortcut`.

`phrases`  

An array of `AppShortcutPhrases` associated with the `AppShortcut`.

`shortTitle`  

A `LocalizedStringResource` representing the short title of the `AppShortcut`.

`systemImageName`  

A `String` representing the system image name for the `AppShortcut`.

`parameterPresentation`  

An `AppShortcutParameterPresentation` object associated with the `AppShortcut`.

## Discussion

Use this initializer to create an App Shortcut for your app intent that people discover in the Shortcuts app and that they can run using the Action button on supported iPhone models.

## See Also

### Creating an app shortcut

init&lt;Intent>(intent: Intent, phrases: [AppShortcutPhrase&lt;Intent>], shortTitle: LocalizedStringResource, systemImageName: String)

Initializes an App Shortcut with phrases that run the app intent, a title, and an image.

init&lt;Intent>(intent: Intent, phrases: [AppShortcutPhrase&lt;Intent>], shortTitle: LocalizedStringResource?, systemImageName: String?)

Initializes an App Shortcut with phrases that run the app intent, a title, and an image.

Deprecated

