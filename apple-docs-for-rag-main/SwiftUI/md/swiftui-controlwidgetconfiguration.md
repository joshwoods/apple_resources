

- SwiftUI
-  ControlWidgetConfiguration 

Protocol

# ControlWidgetConfiguration

A type that describes a control widget’s content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
protocol ControlWidgetConfiguration
```

## Overview

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Associated Types

associatedtype Body : ControlWidgetConfiguration

The type of control widget configuration representing the body of this configuration.

**Required**

### Instance Properties

var body: Self.Body

The content and behavior of the control.

**Required**

### Instance Methods

func description(LocalizedStringResource) -> some ControlWidgetConfiguration

Sets the description shown for the control when a user adds or edits it, using the specified string.

func displayName(LocalizedStringResource) -> some ControlWidgetConfiguration

Sets the name shown for the control when a user adds or edits it, using the specified string.

func promptsForUserConfiguration() -> some ControlWidgetConfiguration

Specifies that a control’s configuration UI should be automatically presented after the widget is added.

func pushHandler(any ControlPushHandler.Type) -> some ControlWidgetConfiguration

Register a type that can handle push tokens changing for controls of this type.

## Relationships

### Conforming Types

- EmptyControlWidgetConfiguration

## See Also

### Composing control widgets

protocol ControlWidget

The configuration and content of a control widget to display in system spaces such as Control Center, the Lock Screen, and the Action Button.

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

func controlWidgetStatus(_:)

The status of the control described by the modified label.

