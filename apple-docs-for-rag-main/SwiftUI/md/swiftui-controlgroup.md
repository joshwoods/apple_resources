

- SwiftUI
-  ControlGroup 

Structure

# ControlGroup

A container view that displays semantically-related controls in a visually-appropriate manner for the context

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
struct ControlGroup where Content : View
```

## Overview

You can provide an optional label to this view that describes its children. This view may be used in different ways depending on the surrounding context. For example, when you place the control group in a toolbar item, SwiftUI uses the label when the group is moved to the toolbar’s overflow menu.

```
ContentView()
    .toolbar(id: "items") {
        ToolbarItem(id: "media") {
            ControlGroup {
                MediaButton()
                ChartButton()
                GraphButton()
            } label: {
                Label("Plus", systemImage: "plus")
            }
        }
    }
```

## Topics

### Creating a control group

init(content: () -> Content)

Creates a new ControlGroup with the specified children

init&lt;C, L>(content: () -> C, label: () -> L)

Creates a new control group with the specified content and a label.

init(_:content:)

Creates a new control group with the specified content that generates its label from a string.

### Creating a control group with an image

init(_:image:content:)

Creates a new control group with the specified content that generates its label from a string and image name.

init(_:systemImage:content:)

Creates a new control group with the specified content that generates its label from a string and image name.

### Creating a configured control group

init(ControlGroupStyleConfiguration)

Creates a control group based on a style configuration.

### Supporting types

struct LabeledControlGroupContent

A view that represents the body of a control group with a specified label.

## Relationships

### Conforms To

- View

## See Also

### Presenting a group of controls

func controlGroupStyle&lt;S>(S) -> some View

Sets the style for control groups within this view.

