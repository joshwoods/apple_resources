

- SwiftUI
-  DismissBehavior 

Structure

# DismissBehavior

Programmatic window dismissal behaviors.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct DismissBehavior
```

## Overview

Use values of this type to control window dismissal during the current transaction.

For example, to dismiss windows showing a modal presentation that would otherwise prohibit dismissal, use the destructive behavior:

```
struct DismissWindowButton: View {
    @Environment(\.dismissWindow) private var dismissWindow

    var body: some View {
        Button("Close Auxiliary Window") {
            withTransaction(\.dismissBehavior, .destructive) {
                dismissWindow(id: "auxiliary")
            }
        }
    }
}
```

## Topics

### Getting behaviors

static let destructive: DismissBehavior

The destructive dismiss behavior.

static let interactive: DismissBehavior

The interactive dismiss behavior.

## Relationships

### Conforms To

- Sendable

## See Also

### Closing windows

var dismissWindow: DismissWindowAction

A window dismissal action stored in a view’s environment.

struct DismissWindowAction

An action that dismisses a window associated to a particular scene.

var dismiss: DismissAction

An action that dismisses the current presentation.

struct DismissAction

An action that dismisses a presentation.

