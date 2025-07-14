

- SwiftUI
-  ControlWidgetTemplate 

Protocol

# ControlWidgetTemplate

A type that describes a control widget’s content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
protocol ControlWidgetTemplate
```

## Overview

Controls are defined using templates in order to ensure that they control will work at all sizes and in all system spaces in which they might be displayed. These templates define images (specifically, symbol images) and text using simple SwiftUI views like Label, Text, and Image; and tint colors using the tint(_:) modifier.

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

associatedtype Body : ControlWidgetTemplate

The type of control widget template representing the body of this template.

**Required**

### Instance Properties

var body: Self.Body

The content and behavior of this control widget.

**Required**

### Instance Methods

func disabled(Bool) -> some ControlWidgetTemplate

Determines whether users can interact with this control widget.

func privacySensitive(Bool) -> some ControlWidgetTemplate

Marks the control template as containing sensitive, private user data.

func tint(Color?) -> some ControlWidgetTemplate

Sets the tint color within this control widget template.

## Relationships

### Conforming Types

- EmptyControlWidgetTemplate

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

struct EmptyControlWidgetTemplate

An empty control widget template.

struct ControlWidgetTemplateBuilder

A custom attribute that constructs a control widget template’s body.

func controlWidgetActionHint(_:)

The action hint of the control described by the modified label.

func controlWidgetStatus(_:)

The status of the control described by the modified label.

