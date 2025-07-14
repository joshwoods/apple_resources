

- SwiftUI
- WidgetConfiguration
-  supportedFamilies(\_:) 

Instance Method

# supportedFamilies(\_:)

Sets the sizes that a widget supports.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
func supportedFamilies(_ families: [WidgetFamily]) -> some WidgetConfiguration
```

## Parameters 

`families`  

The set of sizes the widget supports.

## Return Value

A widget configuration that supports the sizes you specify.

## See Also

### Setting the appearance

func contentMarginsDisabled() -> some WidgetConfiguration

Disable default content margins.

func disfavoredLocations([WidgetLocation], for: [WidgetFamily]) -> some WidgetConfiguration

Sets the disfavored locations for a widget.

func containerBackgroundRemovable(Bool) -> some WidgetConfiguration

A modifier that marks the background of a widget as removable.

