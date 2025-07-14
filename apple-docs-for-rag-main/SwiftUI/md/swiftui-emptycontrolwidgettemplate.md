

- SwiftUI
-  EmptyControlWidgetTemplate 

Structure

# EmptyControlWidgetTemplate

An empty control widget template.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @frozen @preconcurrency
struct EmptyControlWidgetTemplate
```

## Topics

### Initializers

init()

## Relationships

### Conforms To

- BitwiseCopyable
- ControlWidgetTemplate
- Copyable

## See Also

### Composing control widgets

protocol ControlWidget

The configuration and content of a control widget to display in system spaces such as Control Center, the Lock Screen, and the Action Button.

protocol ControlWidgetConfiguration

A type that describes a control widget’s content.

struct EmptyControlWidgetConfiguration

An empty control widget configuration.

struct ControlWidgetConfigurationBuilder

A custom attribute that constructs a control widget’s body.

protocol ControlWidgetTemplate

A type that describes a control widget’s content.

struct ControlWidgetTemplateBuilder

A custom attribute that constructs a control widget template’s body.

func controlWidgetActionHint(_:)

The action hint of the control described by the modified label.

func controlWidgetStatus(_:)

The status of the control described by the modified label.

