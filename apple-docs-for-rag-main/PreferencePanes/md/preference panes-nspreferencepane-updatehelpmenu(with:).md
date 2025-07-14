

- Preference Panes
- NSPreferencePane
-  updateHelpMenu(with:) 

Instance Method

# updateHelpMenu(with:)

Updates the help menu.

Mac Catalyst 14.0+macOS 10.1+

``` source
func updateHelpMenu(with inArrayOfMenuItems: [[String : String]]?)
```

## Discussion

Call this method if you need to update help menu items dynamically. If you have static help menu items, you should not use this method. Specify them under the `NSPrefPanelHelpAnchors` key in the bundle’s `Info.plist` instead.

The array contains dictionaries with two keys. Use NSPreferencePane for the help menu item title, and NSPreferencePane for the anchor reference for `AHLookupAnchor`.

