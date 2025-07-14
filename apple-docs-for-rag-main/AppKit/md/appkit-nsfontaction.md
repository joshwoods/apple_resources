

- AppKit
-  NSFontAction 

Enumeration

# NSFontAction

Actions that modify a font.

macOS

``` source
enum NSFontAction
```

## Topics

### Constants

case noFontChangeAction

No action; the font is returned unchanged.

case viaPanelFontAction

Converts the font according to the `NSFontPanel` method `panelConvertFont:`.

case addTraitFontAction

Converts the font to have an additional trait using convert(_:toHaveTrait:).

case sizeUpFontAction

Converts the font to a larger size using convert(_:toSize:).

case sizeDownFontAction

Converts the font to a smaller size using convert(_:toSize:).

case heavierFontAction

Converts the font to a heavier weight using convertWeight(_:of:).

case lighterFontAction

Converts the font to a lighter weight using convertWeight(_:of:).

case removeTraitFontAction

Converts the font to remove a trait using convert(_:toNotHaveTrait:).

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

