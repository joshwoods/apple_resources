

- Notification Center
- NCWidgetController
-  setHasContent(\_:forWidgetWithBundleIdentifier:) Deprecated

Instance Method

# setHasContent(\_:forWidgetWithBundleIdentifier:)

Sets whether the specified widget has content to display.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 8.0–14.0DeprecatedmacOS 10.10–11.0Deprecated

``` source
func setHasContent(
    _ flag: Bool,
    forWidgetWithBundleIdentifier bundleID: String
)
```

Deprecated

Use WidgetKit instead.

## Parameters 

`flag`  

Indicates whether the widget has content to display. Default value is true.

`bundleID`  

The bundle identifier of the widget.

## Discussion

Both a widget and its containing app can use this method to specify whether the widget has content to display. The value of `flag` determines whether a widget should be visible in the Today view and whether the widget’s most recent snapshot is still valid.

