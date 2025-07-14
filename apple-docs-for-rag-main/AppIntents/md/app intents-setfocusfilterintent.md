

- App Intents
-  SetFocusFilterIntent 

Protocol

# SetFocusFilterIntent

An interface for providing an app intent that you use to adapt your app’s behavior when Focus changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol SetFocusFilterIntent : AppIntent, InstanceDisplayRepresentable
```

## Overview

Related sessions from WWDC22

Session 10121: Meet Focus filters.

## Topics

### Getting the current app configuration

static var current: Self

static func suggestedFocusFilters(for: FocusFilterSuggestionContext) async -> [Self]

You can implement this method to return a list of suggested focus configurations. This is useful when the suggested focus configurations are different from the configuration when the focus is turned off.

**Required** Default implementation provided.

### Configuring app context for the Focus

var appContext: FocusFilterAppContext

An app context that is associated with the focus configuration. The system will retrieve this app context and adapt the system behavior based on the context provided.

**Required** Default implementation provided.

static func invalidateFocusFilterAppContext()

## Relationships

### Inherits From

- AppIntent
- CustomLocalizedStringResourceConvertible
- InstanceDisplayRepresentable
- PersistentlyIdentifiable
- Sendable

## See Also

### Focus filters

Defining your app’s Focus filter

Customize your app’s behavior to reflect the device’s current Focus.

struct FocusFilterAppContext

A type that contains app-specific contextual information for a particular Focus, such as the notification filter criteria to apply.

struct FocusFilterSuggestionContext

A type you use to suggest app configurations for a given Focus.

