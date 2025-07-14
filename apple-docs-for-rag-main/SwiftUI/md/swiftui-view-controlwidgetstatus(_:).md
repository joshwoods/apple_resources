

- SwiftUI
- View
-  controlWidgetStatus(\_:) 

Instance Method

# controlWidgetStatus(\_:)

The status of the control described by the modified label.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func controlWidgetStatus(_ status: Text) -> some View
```

Show all declarations

## Parameters 

`status`  

The status to display.

## Discussion

This text will appear in Control Center when your control’s state changes. You can customize the text by applying this modifier to the control’s value label:

```
// Status Text: "Do Not Disturb Until This Evening" / "Do Not Disturb Disabled"
ControlWidgetToggle("Do Not Disturb", ...) { isOn in
    Image(systemName: "moon")
        .controlWidgetStatus(isOn ? "Do Not Disturb Until This Evening" : "Do Not Disturb Disabled")
}
```

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

struct EmptyControlWidgetTemplate

An empty control widget template.

struct ControlWidgetTemplateBuilder

A custom attribute that constructs a control widget template’s body.

func controlWidgetActionHint(_:)

The action hint of the control described by the modified label.

