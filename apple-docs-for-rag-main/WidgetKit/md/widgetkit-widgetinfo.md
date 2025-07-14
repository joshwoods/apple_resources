

- WidgetKit
-  WidgetInfo 

Structure

# WidgetInfo

A structure that contains information about user-configured widgets.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@preconcurrency
struct WidgetInfo
```

## Mentioned in 

Making a configurable widget

## Topics

### Getting Configured Widget Information

let kind: String

The string specified during creation of the widget’s configuration.

let family: WidgetFamily

The size of the widget: small, medium, or large.

let configuration: INIntent?

A SiriKit intent that contains user-edited values.

### Identifying Widget Information

var id: WidgetInfo

The stable identity of the widget.

### Instance Methods

func widgetConfigurationIntent&lt;Intent>(of: Intent.Type) -> Intent?

Gets the associated App Intent.

### Default Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Configurable widgets

Making a configurable widget

Give people the option to customize their widgets by adding a custom app intent to your project.

Migrating widgets from SiriKit Intents to App Intents

Configure your widgets for backward compatibility.

struct AppIntentConfiguration

An object describing the content of a widget that uses a custom intent to provide user-configurable options.

struct AppIntentRecommendation

An object that describes a recommended intent configuration for a user-customizable widget.

struct IntentConfiguration

An object describing the content of a widget that uses a custom intent definition to provide user-configurable options.

struct IntentRecommendation

An object that describes a recommended intent configuration for a user-customizable widget.

