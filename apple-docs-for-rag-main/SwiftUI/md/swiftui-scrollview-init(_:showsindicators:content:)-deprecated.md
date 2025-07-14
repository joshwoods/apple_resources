

- SwiftUI
- ScrollView
-  init(\_:showsIndicators:content:) Deprecated

Initializer

# init(\_:showsIndicators:content:)

Creates a new instance that’s scrollable in the direction of the given axis and can show indicators while scrolling.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
init(
    _ axes: Axis.Set = .vertical,
    showsIndicators: Bool = true,
    @ViewBuilder content: () -> Content
)
```

Deprecated

Use the ScrollView(\_:content:) initializer and the scrollIndicators(:\_) modifier

## Parameters 

`axes`  

The scroll view’s scrollable axis. The default axis is the vertical axis.

`showsIndicators`  

A Boolean value that indicates whether the scroll view displays the scrollable component of the content offset, in a way suitable for the platform. The default value for this parameter is `true`.

`content`  

The view builder that creates the scrollable view.

## See Also

### Creating a scroll view

init(Axis.Set, content: () -> Content)

Creates a new instance that’s scrollable in the direction of the given axis and can show indicators while scrolling.

