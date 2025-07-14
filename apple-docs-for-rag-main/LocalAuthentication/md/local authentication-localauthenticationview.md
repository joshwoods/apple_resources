

- Local Authentication
-  LocalAuthenticationView 

Structure

# LocalAuthenticationView

A SwiftUI view that displays an authentication interface.

LocalAuthenticationSwiftUImacOS 13.0+

``` source
@MainActor @preconcurrency
struct LocalAuthenticationView where Label : View
```

## Overview

Use a LocalAuthenticationView to display a view that prompts users to authenticate with the app. The view visually represents the state of an LAPolicy evaluation from the Local Authentication framework.

The following shows a LocalAuthenticationView in a Mac app with an implicit LAContext instance:

```
var body: some View {
    LocalAuthenticationView(
        "Continue with Touch ID",
        reason: Text("Access sandcastle competition designs")
    ) { result in
        switch result {
        case .success:
            print("Authorized")
        case .failure(let error):
            print("Authorization failed: \(error)")
        }
    }
    .controlSize(.large)
}
```

If your app’s authorization flow reuses an existing LAContext, pass it as part of initializing a LocalAuthenticationView and call its evaluatePolicy(_:localizedReason:reply:) method after the view appears.

## Topics

### Authenticating with an implicit context

init(reason: Text, context: LAContext?, result: (Result&lt;Void, any Error>) -> Void, label: () -> Label)

Creates a local authentication view.

init&lt;S>(S, reason: Text, context: LAContext?, result: (Result&lt;Void, any Error>) -> Void)

Creates a local authentication view with a title.

init(LocalizedStringKey, reason: Text, context: LAContext?, result: (Result&lt;Void, any Error>) -> Void)

Creates a local authentication view with a localizable title.

init(Text, reason: Text, context: LAContext?, result: (Result&lt;Void, any Error>) -> Void)

Creates a local authentication view with a title text view.

### Authenticating with a context you supply

init&lt;S>(S, context: LAContext)

Creates a local authentication view with a required context.

init(context: LAContext, label: () -> Label)

Creates a local authentication view with a label and required context.

init(LocalizedStringKey, context: LAContext)

Creates a local authentication view with a localizable title and required context.

## Relationships

### Conforms To

- Sendable
- View

