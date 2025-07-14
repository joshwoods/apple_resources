

- App Intents
-  ShortcutsLink 

Structure

# ShortcutsLink

A button that brings users to the current app’s App Shortcuts page in the Shortcuts app.

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
struct ShortcutsLink
```

## Overview

You can create a button by calling the initializer with an additional closure, which gets called whenever the button is tapped before opening the Shortcuts app.

```
ShortcutsLink(action: handleTap)
    .shortcutsLinkStyle(.black)
```

## Topics

### Initializers

init(action: () -> Void)

Creates a link that launches Shortcuts and then executes the specified closure.

### Instance Properties

var body: some View

The content and behavior of the view.

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Buttons

class ShortcutsUIButton

A button that opens the current app’s page in the Shortcuts app.

struct ShortcutsLinkStyle

The styles to apply to buttons you use to open your app’s page in the Shortcuts app.

