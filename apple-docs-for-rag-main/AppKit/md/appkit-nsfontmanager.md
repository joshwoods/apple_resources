

- AppKit
-  NSFontManager 

Class

# NSFontManager

The center of activity for the font-conversion system.

macOS

``` source
class NSFontManager
```

## Overview

The font manager records the currently selected font, updates the Font panel and Font menu to reflect the selected font, initiates font changes, and converts fonts in response to requests from text-bearing objects. In a more prosaic role, NSFontManager can be queried for the fonts available to the application and for the particular attributes of a font, such as whether it’s condensed or extended.

You typically set up a font manager and the Font menu using Interface Builder. However, you can also do so programmatically by getting the shared font manager instance and having it create the standard Font menu at runtime:

```
NSFontManager *fontManager = [NSFontManager sharedFontManager];
NSMenu *fontMenu = [fontManager fontMenu:YES];
```

You can then add the Font menu to your app’s main menu. After the Font menu is installed, your app automatically gains the functionality of both the Font menu and the Font panel.

Font collections are managed by NSFontManager.

## Topics

### Getting the Shared Font Manager

class var shared: NSFontManager

Returns the shared instance of the font manager for the application, creating it if necessary.

### Changing the Default Font Conversion Classes

class func setFontManagerFactory(AnyClass?)

Sets the class that creates the shared font manager object.

class func setFontPanelFactory(AnyClass?)

Sets the class that creates the shared Font panel object.

### Getting Available Fonts

var availableFonts: [String]

The names of the fonts available in the system (not the NSFont objects themselves).

var availableFontFamilies: [String]

The names of the font families available in the system.

func availableFontNames(with: NSFontTraitMask) -> [String]?

Returns the names of the fonts available in the system whose traits are described exactly by the given font trait mask (not the `NSFont` objects themselves).

func availableMembers(ofFontFamily: String) -> [[Any]]?

Returns an array with one entry for each available member of a font family.

### Setting and Examining the Selected Font

func setSelectedFont(NSFont, isMultiple: Bool)

Records the specified font as the currently selected font and updates the Font panel.

var selectedFont: NSFont?

The currently selected font object.

var isMultiple: Bool

A Boolean value that indicates whether the currently selected font has multiple fonts.

func sendAction() -> Bool

A Boolean value that indicates whether a responder handled the font manager’s action message.

func localizedName(forFamily: String, face: String?) -> String

Returns a localized string with the name of the specified font family and face, if one exists.

### Sending Action Methods

func addFontTrait(Any?)

Adds a trait to the font.

func removeFontTrait(Any?)

Removes a trait from the font.

func modifyFont(Any?)

Modifies a trait of the font.

func modifyFontViaPanel(Any?)

Modifies a font trait using input from the Font panel.

func orderFrontStylesPanel(Any?)

Opens the Font Styles panel.

func orderFrontFontPanel(Any?)

Opens the Font panel, creating it if necessary, and displays that panel in front of the app’s windows.

enum NSFontAction

Actions that modify a font.

### Converting Fonts Automatically

func convert(NSFont) -> NSFont

Converts the given font according to the object that initiated a font change, typically the Font panel or Font menu.

### Converting Fonts Manually

func convert(NSFont, toFace: String) -> NSFont?

Returns a font whose traits are as similar as possible to those of the given font except for the typeface, which is changed to the given typeface.

func convert(NSFont, toFamily: String) -> NSFont

Returns a font whose traits are as similar as possible to those of the given font except for the font family, which is changed to the given family.

func convert(NSFont, toHaveTrait: NSFontTraitMask) -> NSFont

Returns a new version of the font object containing a single additional trait.

func convert(NSFont, toNotHaveTrait: NSFontTraitMask) -> NSFont

Returns a new version of a font object without the specified traits.

func convert(NSFont, toSize: CGFloat) -> NSFont

Returns a font object whose traits are the same as those of the given font, except for the size, which is changed to the given size.

func convertWeight(Bool, of: NSFont) -> NSFont

Returns a font object whose weight is greater or lesser than that of the given font.

var currentFontAction: NSFontAction

The current font conversion action.

func convertFontTraits(NSFontTraitMask) -> NSFontTraitMask

Converts font traits to a new traits mask value.

### Getting a Particular Font

func font(withFamily: String, traits: NSFontTraitMask, weight: Int, size: CGFloat) -> NSFont?

Attempts to load a font with the specified characteristics.

### Examining Fonts

func traits(of: NSFont) -> NSFontTraitMask

Returns the traits of the given font.

func fontNamed(String, hasTraits: NSFontTraitMask) -> Bool

Indicates whether the given font has all the specified traits.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

func weight(of: NSFont) -> Int

Returns an approximation of the specified font’s weight.

### Managing the Font Panel and Font Menu

var isEnabled: Bool

A Boolean value that indicates whether the font conversion system’s Font panel and Font menu items are enabled.

func fontPanel(Bool) -> NSFontPanel?

Returns the application’s shared Font panel object, creating it if necessary.

func setFontMenu(NSMenu)

Records the given menu as the application’s Font menu.

func fontMenu(Bool) -> NSMenu?

Returns the menu that’s connected to the font conversion system, creating it if necessary.

### Accessing the Action Property

var action: Selector

The action sent to the first responder when the user selects a new font from the Font panel or chooses a command from the Font menu.

var target: AnyObject?

The object that receives action messages related to the font manager.

### Setting Attributes

func setSelectedAttributes([String : Any], isMultiple: Bool)

Informs the Font panel that the specified font attributes changed for the selected text.

func convertAttributes([String : Any]) -> [String : Any]

Converts attributes in response to an object initiating an attribute change, typically the Font panel or Font menu.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSMenuItemValidation
- NSObjectProtocol

## See Also

### Management

class NSFontCollection

A font collection, which is a group of font descriptors taken together as a single object.

class NSMutableFontCollection

A mutable collection of font descriptors taken together as a single object.

struct NSFontCollectionOptions

Constants that support font collection management.

