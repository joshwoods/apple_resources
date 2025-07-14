

- SwiftUI
- Toggle
-  init(\_:systemImage:sources:isOn:) 

Initializer

# init(\_:systemImage:sources:isOn:)

Creates a toggle representing a collection of values that generates its label from a localized string key and system image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    systemImage: String,
    sources: C,
    isOn: KeyPath>
) where C : RandomAccessCollection
```

Available when `Label` is `Label`.

Show all declarations

## Parameters 

`titleKey`  

The key for the toggle’s localized title, that describes the purpose of the toggle.

`systemImage`  

The name of the image resource to lookup.

`sources`  

A collection of values used as the source for rendering the Toggle’s state.

`isOn`  

The key path of the values that determines whether the toggle is on, mixed or off.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See `Text` for more information about localizing strings.

The following example creates a single toggle that represents the state of multiple alarms:

```
struct Alarm: Hashable, Identifiable {
    var id = UUID()
    var isOn = false
    var name = ""
}

@State private var alarms = [
    Alarm(isOn: true, name: "Morning"),
    Alarm(isOn: false, name: "Evening")
]

Toggle("Enable all alarms", sources: $alarms, isOn: \.isOn)
```

## See Also

### Creating a toggle for a collection

init(_:sources:isOn:)

Creates a toggle representing a collection of values that generates its label from a localized string key.

init&lt;C>(sources: C, isOn: KeyPath&lt;C.Element, Binding&lt;Bool>>, label: () -> Label)

Creates a toggle representing a collection of values with a custom label.

init(_:image:sources:isOn:)

Creates a toggle representing a collection of values that generates its label from a localized string key and image resource.

