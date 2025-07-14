

- SwiftUI
-  ToggleStyle 

Protocol

# ToggleStyle

The appearance and behavior of a toggle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
protocol ToggleStyle
```

## Overview

To configure the style for a single Toggle or for all toggle instances in a view hierarchy, use the toggleStyle(_:) modifier. You can specify one of the built-in toggle styles, like switch or button:

```
Toggle(isOn: $isFlagged) {
    Label("Flag", systemImage: "flag.fill")
}
.toggleStyle(.button)
```

Alternatively, you can create and apply a custom style.

### Custom styles

To create a custom style, declare a type that conforms to the `ToggleStyle` protocol and implement the required makeBody(configuration:) method. For example, you can define a checklist toggle style:

```
struct ChecklistToggleStyle: ToggleStyle {
    func makeBody(configuration: Configuration) -> some View {
        // Return a view that has checklist appearance and behavior.
    }
}
```

Inside the method, use the `configuration` parameter, which is an instance of the ToggleStyleConfiguration structure, to get the label and a binding to the toggle state. To see examples of how to use these items to construct a view that has the appearance and behavior of a toggle, see makeBody(configuration:).

To provide easy access to the new style, declare a corresponding static variable in an extension to `ToggleStyle`:

```
extension ToggleStyle where Self == ChecklistToggleStyle {
    static var checklist: ChecklistToggleStyle { .init() }
}
```

You can then use your custom style:

```
Toggle(activity.name, isOn: $activity.isComplete)
    .toggleStyle(.checklist)
```

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

### Getting built-in toggle styles

static var automatic: DefaultToggleStyle

The default toggle style.

static var button: ButtonToggleStyle

A toggle style that displays as a button with its label as the title.

static var checkbox: CheckboxToggleStyle

A toggle style that displays a checkbox followed by its label.

static var `switch`: SwitchToggleStyle

A toggle style that displays a leading label and a trailing switch.

### Creating custom toggle styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a toggle.

**Required**

struct ToggleStyleConfiguration

The properties of a toggle instance.

typealias Configuration

The properties of a toggle instance.

associatedtype Body : View

A view that represents the appearance and interaction of a toggle.

**Required**

### Supporting types

struct DefaultToggleStyle

The default toggle style.

struct ButtonToggleStyle

A toggle style that displays as a button with its label as the title.

struct CheckboxToggleStyle

A toggle style that displays a checkbox followed by its label.

struct SwitchToggleStyle

A toggle style that displays a leading label and a trailing switch.

## Relationships

### Conforming Types

- ButtonToggleStyle
- CheckboxToggleStyle
- DefaultToggleStyle
- SwitchToggleStyle

## See Also

### Styling toggles

func toggleStyle&lt;S>(S) -> some View

Sets the style for toggles in a view hierarchy.

struct ToggleStyleConfiguration

The properties of a toggle instance.

