

- App Intents
-  SiriTipView 

Structure

# SiriTipView

A SwiftUI view that displays the phrase someone uses to invoke an App Shortcut.

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct SiriTipView
```

## Overview

Use a SiriTipView to display the spoken phrase for the intent you specify. Include an instance of your intent when you create the view, and bind the view to a Boolean to handle the view’s presentation. The following example shows how to configure a button for a reorder intent and bind it to an `isVisible` variable.

```
SiriTipView(intent: ReorderIntent(), isVisible: $isVisible)
    .siriTipViewStyle(.black)
```

Note that you must use the AppIntent in an AppShortcut. Otherwise this will display an empty view.

## Topics

### Creating the view

init&lt;Intent>(intent: Intent, isVisible: Binding&lt;Bool>?)

Creates a `SiriTipView` for the associated action that displays when the binding to a Boolean value is true .

### Implementing the view

var body: some View

The content and behavior of the view.

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Tip views

class SiriTipUIView

A view that displays the phrase a person uses to invoke an App Shortcut.

struct SiriTipViewStyle

The styles to apply to the tip views you use to display spoken phrases.

