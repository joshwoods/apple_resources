

- App Intents
- AppShortcut
-  init(intent:phrases:shortTitle:systemImageName:) 

Initializer

# init(intent:phrases:shortTitle:systemImageName:)

Initializes an App Shortcut with phrases that run the app intent, a title, and an image.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    intent: Intent,
    phrases: [AppShortcutPhrase],
    shortTitle: LocalizedStringResource,
    systemImageName: String
) where Intent : AppIntent
```

## Mentioned in 

Creating your first app intent

## Discussion

Use this initializer to create an App Shortcut for your app intent that people discover in the Shortcuts app and that they can run using the Action button on supported iPhone models.

## See Also

### Creating an app shortcut

init&lt;Intent, Value, Parameter, ParameterKeyPath>(intent: Intent, phrases: [AppShortcutPhrase&lt;Intent>], shortTitle: LocalizedStringResource, systemImageName: String, parameterPresentation: AppShortcutParameterPresentation&lt;Intent, Value, Parameter, ParameterKeyPath>)

Initializes an App Shortcut with phrases that run the app intent, a title, an image, and specified parameters.

init&lt;Intent>(intent: Intent, phrases: [AppShortcutPhrase&lt;Intent>], shortTitle: LocalizedStringResource?, systemImageName: String?)

Initializes an App Shortcut with phrases that run the app intent, a title, and an image.

Deprecated

