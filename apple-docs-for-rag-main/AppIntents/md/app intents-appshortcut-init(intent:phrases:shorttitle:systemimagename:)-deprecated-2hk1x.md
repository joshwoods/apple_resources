

- App Intents
- AppShortcut
-  init(intent:phrases:shortTitle:systemImageName:) Deprecated

Initializer

# init(intent:phrases:shortTitle:systemImageName:)

Initializes an App Shortcut with phrases that run the app intent, a title, and an image.

iOS 16.0–17.0DeprecatediPadOS 16.0–17.0DeprecatedMac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+watchOS 9.0–10.0Deprecated

``` source
init(
    intent: Intent,
    phrases: [AppShortcutPhrase],
    shortTitle: LocalizedStringResource? = nil,
    systemImageName: String? = nil
) where Intent : AppIntent
```

Deprecated

Please provide a shortTitle and systemImageName

## Discussion

Use this initializer to create an App Shortcut for your app intent that people discover in the Shortcuts app and that they can run using the Action button on supported iPhone models.

## See Also

### Creating an app shortcut

init&lt;Intent>(intent: Intent, phrases: [AppShortcutPhrase&lt;Intent>], shortTitle: LocalizedStringResource, systemImageName: String)

Initializes an App Shortcut with phrases that run the app intent, a title, and an image.

init&lt;Intent, Value, Parameter, ParameterKeyPath>(intent: Intent, phrases: [AppShortcutPhrase&lt;Intent>], shortTitle: LocalizedStringResource, systemImageName: String, parameterPresentation: AppShortcutParameterPresentation&lt;Intent, Value, Parameter, ParameterKeyPath>)

Initializes an App Shortcut with phrases that run the app intent, a title, an image, and specified parameters.

