

- SwiftUI
-  ToggleStyleConfiguration 

Structure

# ToggleStyleConfiguration

The properties of a toggle instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ToggleStyleConfiguration
```

## Overview

When you define a custom toggle style by creating a type that conforms to the ToggleStyle protocol, you implement the makeBody(configuration:) method. That method takes a `ToggleStyleConfiguration` input that has the information you need to define the behavior and appearance of a Toggle.

The configuration structure’s label reflects the toggle’s content, which might be the value that you supply to the `label` parameter of the init(isOn:label:) initializer. Alternatively, it could be another view that SwiftUI builds from an initializer that takes a string input, like init(_:isOn:). In either case, incorporate the label into the toggle’s view to help the user understand what the toggle does. For example, the built-in switch style horizontally stacks the label with the control element.

The structure’s isOn property provides a Binding to the state of the toggle. Adjust the appearance of the toggle based on this value. For example, the built-in button style fills the button’s background when the property is `true`, but leaves the background empty when the property is `false`. Change the value when the user performs an action that’s meant to change the toggle, like the button does when tapped or clicked by the user.

## Topics

### Getting the label view

let label: ToggleStyleConfiguration.Label

A view that describes the effect of switching the toggle between states.

struct Label

A type-erased label of a toggle.

### Managing the toggle state

var isMixed: Bool

Whether the Toggle is currently in a mixed state.

var isOn: Bool

A binding to a state property that indicates whether the toggle is on.

var $isOn: Binding&lt;Bool>

## See Also

### Styling toggles

func toggleStyle&lt;S>(S) -> some View

Sets the style for toggles in a view hierarchy.

protocol ToggleStyle

The appearance and behavior of a toggle.

