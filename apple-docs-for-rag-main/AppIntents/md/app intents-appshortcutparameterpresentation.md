

- App Intents
-  AppShortcutParameterPresentation 

Structure

# AppShortcutParameterPresentation

Describes the presentation of an App Shortcut for the provided parameter.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct AppShortcutParameterPresentation where Intent : AppIntent, Value : _IntentValue, Value : Sendable, Parameter : IntentParameter, ParameterKeyPath : KeyPath
```

## Topics

### Initializers

init(for: ParameterKeyPath, summary: AppShortcutParameterPresentationSummary&lt;Intent, Value, Parameter, ParameterKeyPath>, optionsCollections: () -> some AppShortcutOptionsCollectionSpecification&lt;Value.UnwrappedType>)

Creates an object that represents the App Shortcut with the specified parameters.

## See Also

### App Shortcut parameter presentation

struct AppShortcutParameterPresentationSummary

The summary of the presentation of an App Shortcut parameter.

struct AppShortcutParameterPresentationSummaryString

struct AppShortcutParameterPresentationTitle

A struct that represents the title of the presentation of an App Shortcut.

Deprecated

struct AppShortcutParameterPresentationTitleStringDeprecated

