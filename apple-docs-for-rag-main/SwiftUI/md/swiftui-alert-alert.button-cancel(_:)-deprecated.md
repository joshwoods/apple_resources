

- SwiftUI
- Alert
- Alert.Button
-  cancel(\_:) Deprecated

Type Method

# cancel(\_:)

Creates an alert button that indicates cancellation, with a system-provided label.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
static func cancel(_ action: (() -> Void)? = {}) -> Alert.Button
```

Deprecated

Use View.alert(\_:isPresented:presenting:actions:) instead.

## Parameters 

`action`  

A closure to execute when the user taps or presses the button.

## Return Value

An alert button that indicates cancellation.

## Discussion

The system automatically chooses locale-appropriate text for the button’s label.

## See Also

### Getting a button

static func `default`(Text, action: (() -> Void)?) -> Alert.Button

Creates an alert button with the default style.

Deprecated

static func cancel(Text, action: (() -> Void)?) -> Alert.Button

Creates an alert button that indicates cancellation, with a custom label.

Deprecated

static func destructive(Text, action: (() -> Void)?) -> Alert.Button

Creates an alert button with a style that indicates a destructive action.

Deprecated

