

- SwiftUI
- Toggle
-  init(\_:systemImage:isOn:) 

Initializer

# init(\_:systemImage:isOn:)

Creates a toggle that generates its label from a localized string key and system image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    systemImage: String,
    isOn: Binding
)
```

Available when `Label` is `Label`.

Show all declarations

## Parameters 

`titleKey`  

The key for the toggle’s localized title, that describes the purpose of the toggle.

`systemImage`  

The name of the image resource to lookup.

`isOn`  

A binding to a property that indicates whether the toggle is on or off.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See `Text` for more information about localizing strings.

## See Also

### Creating a toggle

init(_:isOn:)

Creates a toggle that generates its label from a localized string key.

init(isOn: Binding&lt;Bool>, label: () -> Label)

Creates a toggle that displays a custom label.

init(_:image:isOn:)

Creates a toggle that generates its label from a localized string key and image resource.

