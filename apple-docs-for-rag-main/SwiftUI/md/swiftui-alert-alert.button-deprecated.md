

- SwiftUI
- Alert
-  Alert.Button Deprecated

Structure

# Alert.Button

A button that represents an operation of an alert presentation.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
struct Button
```

Deprecated

Use a View modifier like alert(_:isPresented:presenting:actions:message:) instead.

## Topics

### Getting a button

static func `default`(Text, action: (() -> Void)?) -> Alert.Button

Creates an alert button with the default style.

static func cancel((() -> Void)?) -> Alert.Button

Creates an alert button that indicates cancellation, with a system-provided label.

static func cancel(Text, action: (() -> Void)?) -> Alert.Button

Creates an alert button that indicates cancellation, with a custom label.

static func destructive(Text, action: (() -> Void)?) -> Alert.Button

Creates an alert button with a style that indicates a destructive action.

