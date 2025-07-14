

- SwiftUI
- WidgetConfiguration
-  containerBackgroundRemovable(\_:) 

Instance Method

# containerBackgroundRemovable(\_:)

A modifier that marks the background of a widget as removable.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
func containerBackgroundRemovable(_ isRemovable: Bool = true) -> some WidgetConfiguration
```

## Parameters 

`isRemovable`  

If `true`, the widget supports removal of the container background in contexts that prefer no backgrounds. If `false`, the system doesn’t remove the background.

## Return Value

A modified widget configuration.

## Discussion

In most cases, mark the background container of a widget as removable to allow people to place the widget in as many contexts as possible. If you mark the background as nonremovable, the widget becomes ineligible in various contexts that require a removable background. For example, a small widget without a removable background doesn’t appear in the widget gallery on the iPad Lock Screen.

If you mark a background as nonremovable, the system always displays the background container of the widget. Note that the background may render differently; for example, it can appear faded or desaturated.

This modifier has no effect on operation system versions prior to iOS 17, watchOS 10, or macOS 14.

## See Also

### Setting the appearance

func supportedFamilies([WidgetFamily]) -> some WidgetConfiguration

Sets the sizes that a widget supports.

func contentMarginsDisabled() -> some WidgetConfiguration

Disable default content margins.

func disfavoredLocations([WidgetLocation], for: [WidgetFamily]) -> some WidgetConfiguration

Sets the disfavored locations for a widget.

