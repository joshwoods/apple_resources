

- Safari Services
- SFSafariToolbarItem
-  setImage(\_:) 

Instance Method

# setImage(\_:)

Sets the image displayed in the toolbar button.

macOS 10.12.4+

``` source
func setImage(_ image: NSImage?)
```

## Parameters 

`image`  

The image to display in the toolbar button.

## Mentioned in 

Adjusting settings for a toolbar item

## Discussion

Pass nil to use the image specified in the `Info.plist` file.

## See Also

### Controlling Toolbar Items

func setEnabled(Bool, withBadgeText: String?)

Sets the enabled state and the badge text for the toolbar item.

Deprecated

func setBadgeText(String?)

Sets the badge text for the toolbar item.

func setEnabled(Bool)

Sets whether the toolbar item is enabled.

func setLabel(String?)

