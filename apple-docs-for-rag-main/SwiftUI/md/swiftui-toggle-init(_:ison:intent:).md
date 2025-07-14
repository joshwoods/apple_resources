

- SwiftUI
- Toggle
-  init(\_:isOn:intent:) 

Initializer

# init(\_:isOn:intent:)

Creates a toggle performing an `AppIntent` and generates its label from a localized string key.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    isOn: Bool,
    intent: some AppIntent
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the toggle’s localized title, that describes the purpose of the toggle.

`isOn`  

Whether the toggle is on or off.

`intent`  

The `AppIntent` to be performed.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See `Text` for more information about localizing strings.

To initialize a toggle with a string variable, use init(_:isOn:intent:) instead.

## See Also

### Creating a toggle for an App Intent

init&lt;I>(isOn: Bool, intent: I, label: () -> Label)

Creates a toggle performing an `AppIntent`.

