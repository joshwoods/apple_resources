

- AppKit
- NSFontAction
-  NSFontAction.heavierFontAction 

Case

# NSFontAction.heavierFontAction

Converts the font to a heavier weight using convertWeight(_:of:).

macOS

``` source
case heavierFontAction
```

## See Also

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

case lighterFontAction

Converts the font to a lighter weight using convertWeight(_:of:).

case removeTraitFontAction

Converts the font to remove a trait using convert(_:toNotHaveTrait:).

