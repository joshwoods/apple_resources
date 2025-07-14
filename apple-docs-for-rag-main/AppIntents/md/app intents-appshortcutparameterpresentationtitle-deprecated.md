

- App Intents
-  AppShortcutParameterPresentationTitle Deprecated

Structure

# AppShortcutParameterPresentationTitle

A struct that represents the title of the presentation of an App Shortcut.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct AppShortcutParameterPresentationTitle where Intent : AppIntent, Value : _IntentValue, Value : Sendable, Parameter : IntentParameter, ParameterKeyPath : KeyPath
```

Deprecated

Please use init(for:summary:optionsCollections:)

## Overview

Provide a specific and a generic title. The specific title should include the parameter in the interpolation. For example provide `"Call \(\.$person)"` as a specific title that includes the parameter and a simple string that doesn’t have the parameter specified, e.g. `"Call Person..."`.

## Topics

### Initializers

init(specific: AppShortcutParameterPresentationTitleString&lt;Intent, Value, Parameter, ParameterKeyPath>, generic: StaticString, table: StaticString?)

Initializes an `AppShortcutParameterPresentationTitle` with the specified parameters.

## See Also

### App Shortcut parameter presentation

struct AppShortcutParameterPresentation

Describes the presentation of an App Shortcut for the provided parameter.

struct AppShortcutParameterPresentationSummary

The summary of the presentation of an App Shortcut parameter.

struct AppShortcutParameterPresentationSummaryString

struct AppShortcutParameterPresentationTitleStringDeprecated

