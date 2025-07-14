

- SwiftUI
-  AlertScene 

Structure

# AlertScene

A scene that renders itself as a standalone alert dialog.

macOS 15.0+

``` source
struct AlertScene where Actions : View, Message : View
```

## Overview

Alert scenes are not attached to any particular window, and present themselves in the center of the current display. The dialog must be dismissed before any further interaction with the app is permitted.

```
@main
struct MyApp: App {
    @State var showLoginAlert = true
    @State var loggedIn = false

    var body: some Scene {
        Window("Welcome User Window", id:"WelcomeWindow") {
            ...
        }
        .defaultLaunchBehavior(loggedIn ? .presented : .suppressed)

        AlertScene("Login Required", isPresented: $showLoginAlert) {
            Button("OK") {
                ...
            }
        }
    }
}
```

All actions present in the ViewBuilder will dismiss the alert. Like the alert modifier, you can determine the role of the buttons with `.cancel` or `.destructive`. If no actions are present, we will automatically include an OK button for dismissal.

## Topics

### Initializers

init(_:isPresented:actions:)

Creates an alert scene with a title and a set of actions.

init(_:isPresented:actions:message:)

Creates an alert scene with a title, a set of actions, and a message.

init(_:isPresented:presenting:actions:)

Creates an alert scene, using the given data to produce the alert’s content with a title, and a set of actions. Note that this creates a text view on your behalf.

init(_:isPresented:presenting:actions:message:)

Creates an alert scene, using the given data to produce the alert’s content with a title, a set of actions, and a message. Note that this creates a text view on your behalf.

## Relationships

### Conforms To

- Scene

## See Also

### Presenting an alert

func alert(_:isPresented:actions:)

Presents an alert when a given condition is true, using a text view for the title.

func alert(_:isPresented:presenting:actions:)

Presents an alert using the given data to produce the alert’s content and a text view as a title.

func alert&lt;E, A>(isPresented: Binding&lt;Bool>, error: E?, actions: () -> A) -> some View

Presents an alert when an error is present.

func alert(_:isPresented:actions:message:)

Presents an alert with a message when a given condition is true using a text view as a title.

func alert(_:isPresented:presenting:actions:message:)

Presents an alert with a message using the given data to produce the alert’s content and a text view for a title.

func alert&lt;E, A, M>(isPresented: Binding&lt;Bool>, error: E?, actions: (E) -> A, message: (E) -> M) -> some View

Presents an alert with a message when an error is present.

