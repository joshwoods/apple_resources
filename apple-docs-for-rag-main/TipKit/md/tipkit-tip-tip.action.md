

- TipKit
- Tip
-  Tip.Action 

Type Alias

# Tip.Action

A type that describes a control associated with a tip.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
typealias Action = Tips.Action
```

## Overview

Use actions to provide additional help and guidance for people looking to get started with your tip. Actions appear at the bottom of your TipView in the form of buttons.

You create an action by providing an `id` and a `title`. The `id` is a string that uniquely identifies the action. The `title` is text that displays as the label on the button.

You can pass a function for the system to call when the action triggers by setting the `perform` attribute in the init(id:title:perform:) initializer. Or you can set the action parameter in the init(_:arrowEdge:action:) initializer of your TipView.

## Topics

### Initializers

## Discussion

init(id: String?, perform: () -> Void, () -> Text)

Creates a tip action that displays a custom label.

init(id: String?, title: some StringProtocol, perform: () -> Void)

Creates a tip action that generates its label from a string.

## See Also

### Providing actions

var actions: [Self.Action]

Buttons that help people get started or learn more about your feature.

**Required**

