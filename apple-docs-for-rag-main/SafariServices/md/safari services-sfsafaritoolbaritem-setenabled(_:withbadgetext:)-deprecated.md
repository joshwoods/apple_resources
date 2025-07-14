

- Safari Services
- SFSafariToolbarItem
-  setEnabled(\_:withBadgeText:) Deprecated

Instance Method

# setEnabled(\_:withBadgeText:)

Sets the enabled state and the badge text for the toolbar item.

macOS 10.12–10.13Deprecated

``` source
func setEnabled(
    _ enabled: Bool,
    withBadgeText badgeText: String?
)
```

Deprecated

use -setEnabled: and -setBadgeText:

## Parameters 

`enabled`  

true to enable the toolbar item; otherwise false.

`badgeText`  

String to display on the badge. Pass `nil` to remove the badge.

## Discussion

The badge text is visible even when the toolbar item is disabled.

## See Also

### Controlling Toolbar Items

func setBadgeText(String?)

Sets the badge text for the toolbar item.

func setEnabled(Bool)

Sets whether the toolbar item is enabled.

func setImage(NSImage?)

Sets the image displayed in the toolbar button.

func setLabel(String?)

