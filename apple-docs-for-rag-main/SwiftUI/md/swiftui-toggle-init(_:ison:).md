

- SwiftUI
- Toggle
-  init(\_:isOn:) 

Initializer

# init(\_:isOn:)

Creates a toggle that generates its label from a localized string key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    isOn: Binding
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the toggle’s localized title, that describes the purpose of the toggle.

`isOn`  

A binding to a property that indicates whether the toggle is on or off.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See `Text` for more information about localizing strings.

## See Also

### Creating a toggle

init(isOn: Binding&lt;Bool>, label: () -> Label)

Creates a toggle that displays a custom label.

init(_:image:isOn:)

Creates a toggle that generates its label from a localized string key and image resource.

init(_:systemImage:isOn:)

Creates a toggle that generates its label from a localized string key and system image.

