

- SwiftUI
-  DismissAction 

Structure

# DismissAction

An action that dismisses a presentation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
struct DismissAction
```

## Overview

Use the dismiss environment value to get the instance of this structure for a given Environment. Then call the instance to perform the dismissal. You call the instance directly because it defines a callAsFunction() method that Swift calls when you call the instance.

You can use this action to:

- Dismiss a modal presentation, like a sheet or a popover.

- Pop the current view from a NavigationStack.

On apps targeting iOS 18 and aligned releases, you also use the dismiss action to pop the implicit stack of a collapsed NavigationSplitView, or clear the equivalent state in an expanded split view.

The specific behavior of the action depends on where you call it from. For example, you can create a button that calls the DismissAction inside a view that acts as a sheet:

```
private struct SheetContents: View {
    @Environment(\.dismiss) private var dismiss

    var body: some View {
        Button("Done") {
            dismiss()
        }
    }
}
```

When you present the `SheetContents` view, someone can dismiss the sheet by tapping or clicking the sheet’s button:

```
private struct DetailView: View {
    @State private var isSheetPresented = false

    var body: some View {
        Button("Show Sheet") {
            isSheetPresented = true
        }
        .sheet(isPresented: $isSheetPresented) {
            SheetContents()
        }
    }
}
```

Be sure that you define the action in the appropriate environment. For example, don’t reorganize the `DetailView` in the example above so that it creates the `dismiss` property and calls it from the sheet(item:onDismiss:content:) view modifier’s `content` closure:

```
private struct DetailView: View {
    @State private var isSheetPresented = false
    @Environment(\.dismiss) private var dismiss // Applies to DetailView.

    var body: some View {
        Button("Show Sheet") {
            isSheetPresented = true
        }
        .sheet(isPresented: $isSheetPresented) {
            Button("Done") {
                dismiss() // Fails to dismiss the sheet.
            }
        }
    }
}
```

If you do this, the sheet fails to dismiss because the action applies to the environment where you declared it, which is that of the detail view, rather than the sheet. In fact, in macOS and iPadOS, if the `DetailView` is the root view of a window, the dismiss action closes the window instead.

The dismiss action has no effect on a view that isn’t currently presented. If you need to query whether SwiftUI is currently presenting a view, read the isPresented environment value.

Note

While the dismiss action can be used to a close window that you create with WindowGroup or Window, prefer DismissWindowAction for that use case instead.

## Topics

### Calling the action

func callAsFunction()

Dismisses the view if it is currently presented.

## Relationships

### Conforms To

- Sendable

## See Also

### Dismissing a presentation

var isPresented: Bool

A Boolean value that indicates whether the view associated with this environment is currently presented.

var dismiss: DismissAction

An action that dismisses the current presentation.

func interactiveDismissDisabled(Bool) -> some View

Conditionally prevents interactive dismissal of presentations like popovers, sheets, and inspectors.

