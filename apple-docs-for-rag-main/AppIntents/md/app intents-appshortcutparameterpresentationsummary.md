

- App Intents
-  AppShortcutParameterPresentationSummary 

Structure

# AppShortcutParameterPresentationSummary

The summary of the presentation of an App Shortcut parameter.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct AppShortcutParameterPresentationSummary where Intent : AppIntent, Value : _IntentValue, Value : Sendable, Parameter : IntentParameter, ParameterKeyPath : KeyPath
```

## Overview

Make sure to provide a summary string that includes the parameter in the interpolation; for example, `"Call \(\.$person)"`.

## Topics

### Initializers

init(AppShortcutParameterPresentationSummaryString&lt;Intent, Value, Parameter, ParameterKeyPath>, table: StaticString?)

Initializes a presentation summary with the specified parameters.

## See Also

### App Shortcut parameter presentation

struct AppShortcutParameterPresentation

Describes the presentation of an App Shortcut for the provided parameter.

struct AppShortcutParameterPresentationSummaryString

struct AppShortcutParameterPresentationTitle

A struct that represents the title of the presentation of an App Shortcut.

Deprecated

struct AppShortcutParameterPresentationTitleStringDeprecated

