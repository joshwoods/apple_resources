

- AppKit
- NSMenu
-  menuBarHeight 

Instance Property

# menuBarHeight

The menu bar height for the main menu in pixels.

macOS

``` source
var menuBarHeight: CGFloat { get }
```

## Discussion

For the main menu, the value of this property is a value of type `CGFloat`, indicating the height of the menu bar in pixels. For any other menu, the value of this property is `0`.

This property supersedes the `menuBarHeight` class method of the `NSMenuView` class.

## See Also

### Managing the Menu Bar

class func menuBarVisible() -> Bool

Returns a Boolean value that indicates whether the menu bar is visible.

class func setMenuBarVisible(Bool)

Sets whether the menu bar is visible and selectable by the user.

