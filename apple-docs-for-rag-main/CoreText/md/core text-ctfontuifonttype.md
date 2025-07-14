

- Core Text
-  CTFontUIFontType 

Enumeration

# CTFontUIFontType

Constants that represent the specific user-interface purpose to specify for font creation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTFontUIFontType
```

## Overview

Use these constants with the CTFontCreateUIFontForLanguage(_:_:_:) function to indicate the intended user interface use of the font reference to be created.

## Topics

### Constants

case none

The user-interface font type isn’t specified.

case user

The default font for documents and other text whose font the user can typically change.

case userFixedPitch

The default font for documents and other text under the user’s control when that font is fixed-pitch.

case system

The system font for standard user-interface items, such as button labels and menu items.

case emphasizedSystem

The system font for emphasis in alerts.

case smallSystem

The standard small system font for informative text in alerts, column headings in lists, help tags, and small controls.

case smallEmphasizedSystem

The small system font for emphasis.

case miniSystem

The standard miniature system font for mini controls and utility window labels and text.

case miniEmphasizedSystem

The miniature system font for emphasis.

case views

The default view font for text in lists and tables.

case application

The default font for text documents.

case label

The font for labels and tick marks on full-size sliders.

case menuTitle

The font for menu titles.

case menuItem

The font for menu items.

case menuItemMark

The font to draw menu-item marks.

case menuItemCmdKey

The font for menu-item command-key equivalents.

case windowTitle

The font for window titles.

case pushButton

The font for a push button, a rounded rectangular button with a text label on it.

case utilityWindowTitle

The font for utility window titles.

case alertHeader

The font for alert headers.

case systemDetail

The standard system font for details.

case emphasizedSystemDetail

The system font for emphasis in details.

case toolbar

The font used for labels of toolbar items.

case smallToolbar

The small font for labels of toolbar items.

case message

The font for standard interface items, such as button labels and menu items.

case palette

The font in tool palettes.

case toolTip

The font for tool tips.

case controlContent

The font for contents of user-interface controls.

### Deprecated

static var kCTFontNoFontType: CTFontUIFontType

The user-interface font type isn’t specified.

Deprecated

static var kCTFontUserFontType: CTFontUIFontType

The font used by default for documents and other text under the user’s control.

Deprecated

static var kCTFontUserFixedPitchFontType: CTFontUIFontType

The font used by default for documents and other text under the user’s control when that font is fixed-pitch.

Deprecated

static var kCTFontSystemFontType: CTFontUIFontType

The system font used for standard user-interface items, such as button labels and menu items.

Deprecated

static var kCTFontEmphasizedSystemFontType: CTFontUIFontType

The system font used for emphasis in alerts.

Deprecated

static var kCTFontSmallSystemFontType: CTFontUIFontType

The standard small system font used for informative text in alerts, column headings in lists, help tags, and small controls.

Deprecated

static var kCTFontSmallEmphasizedSystemFontType: CTFontUIFontType

The small system font used for emphasis.

Deprecated

static var kCTFontMiniSystemFontType: CTFontUIFontType

The standard miniature system font used for mini controls and utility window labels and text.

Deprecated

static var kCTFontMiniEmphasizedSystemFontType: CTFontUIFontType

The miniature system font used for emphasis.

Deprecated

static var kCTFontViewsFontType: CTFontUIFontType

The view font used as the default font of text in lists and tables.

Deprecated

static var kCTFontApplicationFontType: CTFontUIFontType

The default font for text documents.

Deprecated

static var kCTFontLabelFontType: CTFontUIFontType

The font used for labels and tick marks on full-size sliders.

Deprecated

static var kCTFontMenuTitleFontType: CTFontUIFontType

The font used for menu titles.

Deprecated

static var kCTFontMenuItemFontType: CTFontUIFontType

The font used for menu items.

Deprecated

static var kCTFontMenuItemMarkFontType: CTFontUIFontType

The font used to draw menu-item marks.

Deprecated

static var kCTFontMenuItemCmdKeyFontType: CTFontUIFontType

The font used for menu-item command-key equivalents.

Deprecated

static var kCTFontWindowTitleFontType: CTFontUIFontType

The font used for window titles.

Deprecated

static var kCTFontPushButtonFontType: CTFontUIFontType

The font used for a push button, a rounded rectangular button with a text label on it.

Deprecated

static var kCTFontUtilityWindowTitleFontType: CTFontUIFontType

The font used for utility window titles.

Deprecated

static var kCTFontAlertHeaderFontType: CTFontUIFontType

The font used for alert headers.

Deprecated

static var kCTFontSystemDetailFontType: CTFontUIFontType

The standard system font used for details.

Deprecated

static var kCTFontEmphasizedSystemDetailFontType: CTFontUIFontType

The system font used for emphasis in details.

Deprecated

static var kCTFontToolbarFontType: CTFontUIFontType

The font used for labels of toolbar items.

Deprecated

static var kCTFontSmallToolbarFontType: CTFontUIFontType

The small font used for labels of toolbar items.

Deprecated

static var kCTFontMessageFontType: CTFontUIFontType

The font used for standard interface items, such as button labels and menu items.

Deprecated

static var kCTFontPaletteFontType: CTFontUIFontType

The font used in tool palettes.

Deprecated

static var kCTFontToolTipFontType: CTFontUIFontType

The font used for tool tips.

Deprecated

static var kCTFontControlContentFontType: CTFontUIFontType

The font used for contents of user-interface controls.

Deprecated

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

typealias CTFontTableTag

Font table tags provide access to font table data.

struct CTFontTableOptions

Constants that describe font table options.

struct CTFontOptions

Options for font creation and descriptor matching.

