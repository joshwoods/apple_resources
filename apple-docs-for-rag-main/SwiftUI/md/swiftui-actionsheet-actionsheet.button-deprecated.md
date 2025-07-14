

- SwiftUI
- ActionSheet
-  ActionSheet.Button Deprecated

Type Alias

# ActionSheet.Button

A button representing an operation of an action sheet presentation.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
typealias Button = Alert.Button
```

Deprecated

Use a View modifier like confirmationDialog(_:isPresented:titleVisibility:presenting:actions:message:) instead.

## Discussion

The ActionSheet button is type-aliased to the Alert button type, which provides default, cancel, and destructive styles.

